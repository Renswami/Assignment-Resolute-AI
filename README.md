# Assignment-Resolute-AI
public class resoluteAIPVTLTDassignment {

	public static void main(String[] args) throws InterruptedException {
		// TODO Auto-generated method stub
		System.setProperty("webdriver.chrome.driver","C:\\Users\\santosh\\Desktop\\selenium with jar\\chromedriver-win64\\chromedriver.exe");
		ChromeOptions option=new ChromeOptions();
		option.addArguments("--remote-allow-origins=*");
		 ChromeDriver driver = new ChromeDriver(option);
		 
		 driver.manage().window().maximize();
		
		driver.navigate().to("https://facegenie-ams-school.web.app/");
		
		Thread.sleep(1000);
		WebElement email = driver.findElement(By.id("email"));
		email.sendKeys("testbams@gmail.com");
		
		Thread.sleep(1000);
		WebElement password = driver.findElement(By.id("password"));
		password.sendKeys("facegenie");
		
		Thread.sleep(1000);
		WebElement login= driver.findElement(By.xpath("//button[@type='submit']"));
		login.click();
		
	    Thread.sleep(18000);
	    driver.quit();
		
        	
		
	}

}
