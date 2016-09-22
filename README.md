# Desk
import javax.swing.*;
import javax.swing.border.TitledBorder;

import java.awt.*;
import java.awt.event.*;
public class MyJPanel extends JFrame{
	private static String path="f:/images/";
	static Icon[] icons={
		new ImageIcon(path + "查看文件按钮.png"),
		new ImageIcon(path + "放大客户端桌面.png"),
		new ImageIcon(path + "黑屏.png"),
		new ImageIcon(path + "进程.png"),
		new ImageIcon(path + "客户端广播.png"),
		new ImageIcon(path + "浏览.png"),
		new ImageIcon(path + "配置.png"),
		new ImageIcon(path + "强制开关机.png"),
		new ImageIcon(path + "全体广播.png"),
		new ImageIcon(path + "视频录像.png"),
		new ImageIcon(path + "搜索文件.png"),
		new ImageIcon(path + "锁客户机.png"),
	};

	JButton jb1=new JButton(new ImageIcon(path + "查看文件按钮.png"));
	JButton jb2=new JButton(new ImageIcon(path + "放大客户端桌面.png"));
	JButton jb3=new JButton(new ImageIcon(path + "黑屏.png"));
	JButton jb4=new JButton(new ImageIcon(path + "进程.png"));
	JButton jb5=new JButton(new ImageIcon(path + "客户端广播.png"));
	JButton jb6=new JButton(new ImageIcon(path +  "浏览.png"));
	JButton jb7=new JButton(new ImageIcon(path + "强制开关机.png"));
	JButton jb8=new JButton(new ImageIcon(path + "全体广播.png"));
	JButton jb9=new JButton(new ImageIcon(path + "视频录像.png"));
	JButton jb10=new JButton();
	JButton jb11=new JButton();
	JButton jb12=new JButton();


	JFrame frame;
	JPanel panel1;
	JPanel panel2;
	JPanel panel3;
	JPanel panel4;
	JPanel panel5;
	JPanel panel6;
	public MyJPanel(){
		frame=new JFrame("远程桌面监控系统");
		panel1=new JPanel();
		panel2=new JPanel();
		panel3=new JPanel();
		panel4=new JPanel();
		panel5=new JPanel();
		panel6=new JPanel();
		panel1.setBackground(Color.CYAN);
		panel2.setBackground(Color.BLACK);
		panel3.setBackground(Color.blue);
		panel4.setBackground(Color.DARK_GRAY);
		panel5.setBackground(Color.GREEN);
		panel6.setBackground(Color.RED);
		
		panel3.setBorder(new TitledBorder("用户列表"));
		panel5.setBorder(new TitledBorder("信息管理"));
		panel6.setBorder(new TitledBorder("用户记录"));
		panel1.add(jb1);
		panel1.add(jb2);
		panel1.add(jb3);
		panel1.add(jb4);
		panel1.add(jb5);
		panel1.add(jb6);
	
		panel3.add(new JTextField(30));
		panel4.add(jb7);
		panel4.add(jb8);
		panel4.add(jb9);
		panel5.add(new JTextField(30));
		panel6.add(new JTextField(30));
		
		Container cp=frame.getContentPane();
		cp.setLayout(null);
		panel1.setSize(1500,200);
		panel2.setSize(50,50);
		panel3.setSize(300,300);
		panel4.setSize(800,300);
		cp.add(panel1,BorderLayout.NORTH);
		cp.add(panel2,BorderLayout.WEST);
		cp.add(panel3,BorderLayout.CENTER);
		cp.add(panel4,BorderLayout.EAST);
		cp.add(panel5,BorderLayout.SOUTH);
		
		panel1.setLayout(new GridLayout(1,5));
		panel2.setLayout(new GridLayout());
		panel3.setLayout(new GridLayout());
		panel4.setLayout(new GridLayout(1,4));
		panel5.setLayout(new GridLayout());
		panel6.setLayout(new GridLayout());
		cp=getContentPane();
		frame.setSize(5000,1500);
		frame.show();
		
	}
public static void main(String[] args){
	new MyJPanel();
	
}
}
