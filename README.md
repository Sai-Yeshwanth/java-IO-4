import java.io.FileOutputStream;
import java.io.IOException;
import java.io.BufferedOutputStream;

public class Jala {
	public static void main(String[] args) throws IOException {
		FileOutputStream fos = new FileOutputStream("myfile.txt");
		BufferedOutputStream bos = new BufferedOutputStream(fos);
		String data = "Hi My name is Sai";
		bos.write(data.getBytes());
		bos.close();
    }
}
