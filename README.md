# Commonprefix

public class commonprefix {
	public static void main(String args[]) {

		String s1 = "Rajesh";
		String s2 = "Ramya";
		
		StringBuffer str = new StringBuffer();
		String s3 = s1.substring(0, 2);
		String s4 = s2.substring(0, 2);
		char c = 0;
		char c1 = 0;
		for (int i = 0; i < s3.length(); i++) {
			c = s3.charAt(i);
			for (int j = 0; j < s4.length(); j++) {
				c1 = s4.charAt(j);
				if (c == c1) {
					str.append(c1);

				}

			}

		}
		if (c != c1) {
			System.out.println("no common prefix");

		}
		System.out.println(str);
	}
}
