# Java-FileOutputStream
创建一个
```java
import java.io.FileOutputStream;
import java.io.IOException;

public class FileOutputStreamDemo {
	public static void main(String[] args) throws IOException {
//		FileOutputStream fos = new FileOutputStream("d:\\a.txt",true);
//		
//		byte [] byt = {65,66,67,68};
//		fos.write("hello\r\n".getBytes());
//		fos.close();
//		
		FileOutputStream fos = null;
		try{
			fos = new FileOutputStream("d:\\a.txt",true);
			fos.write("world".getBytes());
		  }catch(IOException ex){
			  System.out.println(ex.getMessage());
		}finally {
			if(fos != null) {
				fos.close();
			}
		}	
	}
}
```
