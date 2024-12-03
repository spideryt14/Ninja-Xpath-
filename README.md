# Ninja-Xpath-
Ninja app registration page automation testing, 
package com.fb;
import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.WebElement;
import org.openqa.selenium.chrome.ChromeDriver;
import java.util.Scanner;

public class Complex {

	public static void main(String[] args) throws InterruptedException
	{
	
		WebDriver test=new ChromeDriver();
		test.get("https://ananinja.com/sa/en");
		test.findElement(By.cssSelector("body > div:nth-child(1) > div:nth-child(1) > div:nth-child(3) > div:nth-child(7)")).click();
		test.findElement(By.xpath("//p[@class='text-base text-gray-300 font-bold leading-4']")).click();
		test.findElement(By.xpath("//input[@placeholder='5XX XXX XXX']")).sendKeys("560665201");
		test.findElement(By.xpath("//button[@type='submit']")).click();
		Thread.sleep(3000);
		test.close();
		
		
		
		
		
	}

}
