# UNIT-CONVERTER
//This is a basic unit converter
#include<stdio.h>
int main()
{
	char category;
	int temp,valuef,valuec;
	float F,degreeC;
	int currency,valueusd,valuejpy,valuermb;
	float EURO,JPY,RMB;
	int mass,Ounce,Gram;
	float Pounds,gtoPounds;
	int length,metre1,metre2;
	float Miles,Yard;
		printf("Welcome to Unit Convertor\n");
		printf("The list of conversions is given below : \n");
		printf("1.Temperature(T)\n2.Currency(C)\n3.Mass(M)\n4.Length(L)\n");
		printf("Please enter the letter that you want to convert :-");
		scanf("%c",&category);
		
		if(category == 'T')
		{
			printf("\nWelcome to temperature  convertor\n");
			printf("Here is a list of conversions to choose from :\n");
			printf("Enter 1 for Fahrenheit to Celcius.\n");
			printf("Enter 2 for Celcius to Fahrenheit.\n");
			scanf("%d",&temp);
			
			if(temp == 1)
			{
				printf("Enter the Fahrenheit degree = \n");
				scanf("%d",&valuef);
				degreeC = ((valuef-32)*(5.0/9.0));
				printf("Celcius = %.2f",degreeC);
			}
			else if(temp == 2)
			{
				printf("Enter the Celcius degree = \n");
				scanf("%d",&valuec);
				F = ((9/5)*valuec + 32);
				printf("Fahrenheit = %.2f",F);
			}
			else
			printf("Please enter the correct choice");
	    }
	    else if(category == 'C')
	    {
	    	printf("\nWelcome to Currency Converter\n");
	    	printf("The list of conversions are given below : \n");
	    	printf("Enter 1 for USD to Euro.\n");
	    	printf("Enter 2 for USD to JPY.\n");
	    	printf("Enter 3 for USD to RMB.\n");
	    	scanf("%d",&currency);
	    	
	    	if(currency == 1)
	    	{
	    		printf("\nEnter the USD amount = ");
	    		scanf("%d",&valueusd);
	    		EURO = valueusd*0.87;
	    		printf("Euro = %.2f ",EURO);
			}
			else if(currency == 2)
			{
				printf("Please enter the USD amount = \n");
				scanf("%d",&valuejpy);
				JPY = valuejpy*111.09;
				printf("JPY = %.2f",JPY);
			}
			else if(currency == 3)
			{
				printf("Enter the USD amount = \n");
				scanf("%d",&valuermb);
				RMB = valuermb*6.82;
				printf("RMB = %.2f",RMB);
			}
			else
			printf("Enter the correct choice");
		}
		else if(category == 'M')
		{
			printf("\nWelcome to Mass Converter\n");
			printf("The list of conversions are given below :\n");
			printf("Enter 1 for ounces to pounds.\n");
			printf("Enter 2 for gram to pounds.\n");
			scanf("%d",&mass);
			
			if(mass == 1)
			{
				printf("Enter the ounce amount = \n");
				scanf("%d",&Ounce);
				Pounds = Ounce*0.0625;
				printf("Pounds = %.2f",Pounds);
			}
			else if(mass == 2)
			{
				printf("Enter the gram amount = \n");
				scanf("%d",&Gram);
				gtoPounds = Gram*0.00220462;
				printf("Pounds = %.2f",gtoPounds);
			}
			else
			printf("Please enter the correct value");
		}
		else if(category == 'L')
		{
		printf("\nWelcome to Length Converter\n");
		printf("The list of conversions are given below :\n");
		printf("Enter 1 for metres to miles.\n");
		printf("Enter 2 for metre to yard.\n");
		scanf("%d",&length);
		
		if(length == 1)
		{
			printf("Enter the value in metre = \n");
			scanf("%d",&metre1);
			Miles = metre1*0.0006214;
			printf("Miles = %.2f",Miles);
		}
		else if(length == 2)
		{
			printf("Enter the value in metre = \n");
			scanf("%d",&metre2);
			Yard = metre2*1.0936;
			printf("Yard = %.2f",Yard);
		}
		else
		printf("Enter the correct value");
    }
}
