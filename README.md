# hackPrinceton-mapaeli-
source code

import javax.swing.JFrame;



public class Main {
	public static void main(String[] args) {
		JFrame main_frame = new JFrame();
		main_frame.setTitle("Mapaeli: the happy map");
		main_frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);

		CommentThread thread = new CommentThread();
		ThreadView tlist_view = new ThreadView(thread);
		main_frame.setContentPane(tlist_view);

		main_frame.pack();
		main_frame.setVisible(true);
	}
}
