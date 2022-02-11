# 6  Digit OTP-Generation code in java 


// If you want to generate 4 digit otp just change the value of i in for loop condition.


package com.company;
import java.util.function.Supplier;
public class Main {

    public static void main(String[] args) {
        Supplier<String> s=()->{
            String otp="";
            for(int i=0;i<6;i++)
            {
                otp=otp+(int)(Math.random()*10);
            }
            return otp;

        };
        System.out.println(s.get());
    }
}

