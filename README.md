public class A {
	
	public static void main(String[] args) throws IOException {
		System.setProperty("webdriver.chrome.driver", "C:\\Users\\balaji\\Desktop\\Java Automation\\1-Jan\\Automation\\chromedriver_win32 (2)\\chromedriver.exe");
		WebDriver driver =new ChromeDriver();		
		driver.get("https://www.facebook.com/");
		driver.manage().window().maximize();
		
		File src = ((TakesScreenshot)driver).getScreenshotAs(OutputType.FILE);
		
		File f = new File("C:\\Users\\balaji\\Desktop\\Java Automation\\1-Jan\\Automation\\screenshot\\image2.jpg");
		
		FileHandler.copy(src, f);
		
		
	}
Just a change
}

