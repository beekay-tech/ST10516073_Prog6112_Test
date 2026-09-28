# ST10516073_Prog6112_Test
/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 */

package com.mycompany.franchisereports;

/**
 *
 * @author Student
 */
import java.util.*;

public class Franchisereports {
//City names
    String[]cities = {
        "Cape Town"
        "Port Elizabeth"
        "Pretoria"
 //gaming console names 
    String [] consoles = {
        "PS5"
        "XBOX"
        "SWITCH"
    //Sales for cities
    int[][] sales ={
        {1000,2000,3000},//Cape town
        {2000,3000,4000},//Port elizabeth
        {1500,1100,1200},//Pretoria
    };
    //sales for   each city
    int[] cityTotals = new int[cities.length]
    // Sales for each city
     for (int i = 0;i <sales.length; i++) {
        for (int j = 0;j < sales[i].length; j++) {
        cityTotal[i] += sales [i][j];
    }
}
     //city with most sales
     int highestSales = cityTotals[0];
      int highestCityIndex =0;
      
     for (int i=1; i< cityTotals.length; i++) {
      if (cityTotals[i]>highestSales){
          highestSales = cityTotals[i];
          highestCityIndex = i;
       }
    }
   //output display
   System.out.println("--------------------------");
   System.out.println("     GAMING  CONSOLE REPORT");
   System.out.println("---------------------------");
}
            
    }

    ##Question 2
    /*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 * Click nbfs://nbhost/SystemFileSystem/Templates/Classes/Class.java to edit this template
 */

/**
 *
 * @author Student
 */
public abstract class Console implements IConsole {
    //variables
    private String consoleType;
    private String store;
    private int totalSales;
    //constructor
    public Consoles(String consoleType, String store, int totalSales){
       this.consoleType = consoleType;
       this.store = store;
       this.totalSales = totalSales;
    }
    
    //consoletype
    public String getconsoleType(){
        return consoleType;
    }
    
    //storename
    public String getStore;
        return store;
    }
    //total sales
    public int getTotalSales;
       return totalSales;
    }   
}

  /**
 *
 * @author Student
 */
public class ConsoleSales extends Consoles {
    
    //constructor
    public ConsoleSales(String consoleType,String store, int totalSales){
        super(consoleType, store, totalSales);
    }
    
    //report
    public void printReport(){
        
        System.out.println("-------------------------------------");
        System.out.println("   CONSOLE SALES REPORT");
        System.out.println("-------------------------------------");
        System.out.println("console type:" + getConsoleType());
        System.out.println("Store Name:" + getStore());
        System.out.println("Total Sales:" + getTotalSales());
        System.out.println("---------------------------------------");
    }  
}
  


    }
}
