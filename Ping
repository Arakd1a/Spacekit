package spacekit;

import java.net.*;
import java.io.*;
import java.util.*;

class Ping {
	public static void main(String[] args) {
		
		Spacepanel callClass = new Spacepanel();
		String hostname = textHostname.getText();


	
        String pingResult = "";

        
        String pingCmd = "ping " + hostname;{ 
        
 try {
            Runtime r = Runtime.getRuntime();
            Process p = r.exec(pingCmd);

            BufferedReader in = new BufferedReader(new
            InputStreamReader(p.getInputStream()));
            String inputLine;
            while ((inputLine = in.readLine()) != null) {
                System.out.println(inputLine);
                pingResult += inputLine;
            }
            in.close();

        } catch (IOException e) {
            System.out.println(e);
        }

}
}}


