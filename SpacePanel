package spacekit;

import java.awt.EventQueue;

import javax.swing.JFrame;
import javax.swing.JTextField;
import java.awt.BorderLayout;
import javax.swing.JButton;
import java.awt.event.ActionListener;
import java.awt.event.ActionEvent;

public class Spacepanel {

	public JFrame frame;
	public static JTextField textHostname;
	

	/**
	 * Launch the application.
	 */
	public static void main(String[] args) {
		EventQueue.invokeLater(new Runnable() {
			public void run() {
				try {
					Spacepanel window = new Spacepanel();
					window.frame.setVisible(true);
				} catch (Exception e) {
					e.printStackTrace();
				}
			}
		});
	}

	/**
	 * Create the application.
	 */
	public Spacepanel() {
		initialize();
	}

	/**
	 * Initialize the contents of the frame.
	 */
	public void initialize() {
		frame = new JFrame();
		frame.setBounds(100, 100, 450, 300);
		frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
		
		textHostname = new JTextField();
		frame.getContentPane().add(textHostname, BorderLayout.NORTH);
		textHostname.setColumns(10);
		
		JButton btnPing = new JButton("PING");
		btnPing.addActionListener(new ActionListener() {
			public void actionPerformed(ActionEvent e) {
				
				String hostname = textHostname.getText();
				new Ping();
				
				
			}
		});
		frame.getContentPane().add(btnPing, BorderLayout.WEST);
		
		
		JButton btnClear = new JButton("Clear");
		btnClear.addActionListener(new ActionListener() {
			public void actionPerformed(ActionEvent arg0) { 
				 textHostname.setText("");	
				
			}
		});
		frame.getContentPane().add(btnClear, BorderLayout.CENTER);
	}

}
