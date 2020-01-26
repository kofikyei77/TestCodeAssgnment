# TestCodeAssgnment
An assignment given to us by Speed
package org.personallearning.org;

import java.util.Scanner;
public class EchoIgniter {
	public static void main(String args []) {
		
		boolean strt_confirm=false;
		String echo_ignitor_strt="start";
		String echo_distinguisher_end="end";
		
		check_kybd_inpt(echo_ignitor_strt);
		extinguish_process(echo_distinguisher_end);
	}
				
		private static void check_kybd_inpt(String echo_ignitor_strt) {
			boolean strt_confirm;
			Scanner kybd_inpt = new Scanner(System.in);
			System.out.println("Enter START to begin the ECHO process: \n");
			String kybd_inpt_temp = kybd_inpt.nextLine();
			
			strt_confirm=true;
					
					while(strt_confirm==true)
					{
						
						if(kybd_inpt_temp.equalsIgnoreCase(echo_ignitor_strt))
						{
							for(int i=0; i<=1000000; i++) {
						System.out.println("Write anythin : ");
						Scanner input = new Scanner(System.in);
						
						String temp=input.nextLine();
						
						System.out.println(temp);
						
					}
				}
						else if(!kybd_inpt_temp.equalsIgnoreCase(echo_ignitor_strt))
						{		
							System.out.println("That was not START\n");
							check_kybd_inpt(echo_ignitor_strt);
						}	
						
						
					}
					}
		
					
			private static void extinguish_process(String echo_distinguisher_end) {
				Scanner kybd_inpt_temp = new Scanner(System.in);
				String temp;
				
				temp=kybd_inpt_temp.nextLine();
				
				if(temp.equalsIgnoreCase(echo_distinguisher_end)) {
					
					System.out.println("THE END!");
			kybd_inpt_temp.close();
			}
	}
}
