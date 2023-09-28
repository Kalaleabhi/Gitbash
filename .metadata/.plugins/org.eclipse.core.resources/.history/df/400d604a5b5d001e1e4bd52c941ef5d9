package com.PracticeTestNG;

import java.time.Duration;

import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.WebElement;
import org.openqa.selenium.chrome.ChromeDriver;
import org.openqa.selenium.chrome.ChromeOptions;
import org.openqa.selenium.edge.EdgeDriver;
import org.openqa.selenium.firefox.FirefoxDriver;
import org.testng.Assert;
import org.testng.annotations.Test;

public class SpicejetTest {
	
	@Test
	public void method()throws Throwable
	{ 
		  ChromeOptions options = new ChromeOptions();
	        options.addArguments("--disable-notifications");

	      
	        WebDriver driver = new ChromeDriver(options);
		driver.manage().window().maximize();
		driver.get("https://www.spicejet.com/");
		String month="October ";
		int date =3;
		Thread.sleep(5000);
		driver.manage().timeouts().implicitlyWait(Duration.ofSeconds(10));
	//	driver.findElement(By.xpath("(//input[@class='css-1cwyjr8 r-homxoj r-ubezar r-10paoce r-13qz1uu'])[1]")).sendKeys("Bangalore");
		Thread.sleep(3000);
	WebElement ele=	driver.findElement(By.xpath("(//input[@class='css-1cwyjr8 r-homxoj r-ubezar r-10paoce r-13qz1uu'])[2]"));
		ele.click();
	ele.sendKeys("Hyderabad");
	Thread.sleep(3000);
	driver.findElement(By.xpath("//div[text()='"+month+"']/../../div[@class='css-1dbjc4n']/div/div[.='"+date+"']")).click();
driver.findElement(By.xpath("(//div[.='Search Flight'])[3]")).click();
String s=driver.findElement(By.xpath("(//div[@class='css-76zvg2 r-homxoj r-1hfyk0a'])[1]")).getText();
System.out.print(s);
Assert.assertTrue(s.contains("One Way"));
Assert.assertTrue(s.contains("Bengaluru"));
Assert.assertTrue(s.contains("Hyderabad"));
Assert.assertTrue(s.contains(" 1 Adult"));
		
	}
	@Test
public void array()
	{
		int arr[]= {20,10,5};
		int b[]=new int[arr.length];
		for(int i=0;i<arr.length;i++)
		{
			System.out.print(arr[i]+" ");
		}
		System.out.println();
		for(int i=0;i<arr.length;i++)
		{
		b[i]=arr[i]*arr[i]*arr[i];
		System.out.print(b[i]+" ");
		}
		System.out.println();
		int temp=0;
		for(int j=0;j<b.length;j++)
		{
			for(int k=j+1;k<b.length;k++)
			{
				if(b[j]>b[k])
				{
					temp=b[j];
					b[j]=b[k];
					b[k]=temp;
				}
			}
		}
		
	for(int a:b)
		{
		System.out.print(a+" ");
		System.out.println();
	}
	String s = "wwwprethe";
	char chr[] = s.toCharArray();
	for (int i = 0; i < chr.length; i++) {
		int count = 1;
		if (chr[i] != ' ') {
			for (int j = i + 1; j < chr.length; j++) {
				if (chr[i] == chr[j]) {
					count++;
					chr[j] = ' ';
				}
			}
			System.out.print(chr[i] +""+ count+" ");
		}
	}

	}
	
}