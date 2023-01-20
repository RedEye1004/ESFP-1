# ESFP-1
#include<stdio.h>
#include<stdlib.h>
int farmer_login()
{       char uname1[20],pass1[20];
        printf("Enter your Username:");
        scanf ("%s",&uname1);
        fflush(stdin);
        printf("Enter your Password:");
        scanf ("%s",&pass1);     
}
int content()
{   
        printf("\n              ===================================================================================================================================");
        printf("\n                                                                      TABLE OF CONTENTS                                                          ");
        printf("\n              ===================================================================================================================================");
        printf("\n");
        printf("\n1.  CONCLUSIONS OF THE WORKSHOP........................................................................................................................................ 7\n");
        printf("\n2.  OPENING ADDRESS ................................................................................................................................................... 13\n");
        printf("\n3.  ADOPTING TECHNOLOGIES FOR SUSTAINABLE FARMING SYSTEMS: \n    AN OECD PERSPECTIVE................................................................................................................................................ 15\n");
        printf("\n4.  ADOPTING TECHNOLOGIES FOR SUSTAINABLE FARMING SYSTEMS: \n    THE FARMERS PERSPECTIVE ........................................................................................................................................... 25\n");
        printf("\n5.  ADOPTING TECHNOLOGIES FOR SUSTAINABLE FARMING SYSTEM: \n     THE PUBLIC INTEREST PERSPECTIVE................................................................................................................................... 29\n");
        printf("\n6.  ASSESSING SUSTAINABLE TECHNOLOGIES IN DEVELOPING COUNTRIES:\n    MEASURING ENVIRONMENTAL, ECONOMIC AND SOCIAL IMPACTS .............................................................................................................. 35\n");
        printf("\n7.  HOW DEVELOPMENTS IN THE AGRO-FOOD CHAIN ARE AFFECTING TECHNOLOGIES AND FARMING SYSTEMS............................................................................. 50\n");
        printf("\n8.  HOW ARE GOVERNMENTS INFLUENCING INNOVATION AND UPTAKE OF TECHNOLOGIES FOR SUSTAINABLE FARMING SYSTEMS:\n    PESTICIDES AND BIOTECHNOLOGY .......................... 61\n");
        printf("\n9.  IMPROVING DISSEMINATION OF TECHNOLOGICAL INFORMATION TO FARMERS?................................................................................................... 92\n");
        printf("\n10. THE ADOPTION OF SUSTAINABLE AGRICULTURAL PRODUCTION PRACTICES:\n    RESULTS FROM THE U.S. DEPARTMENT OF AGRICULTURE AREA STUDIES PROJECT .............................................................................................. 98\n");
        printf("\n11. POLICY-TECHNOLOGY INTERACTIONS FOR INTENSIVE FARMING SYSTEMS:\nSOME EXPERIENCES FROM THE NETHERLANDS.................................................................................................................................. 109\n");
        printf("\n12. EVOLUTION AND INSTRUMENTS FOR THE IMPLEMENTATION OF A WHOLE FARM ENVIRONMENTAL MANAGEMENT PROGRAMME IN SWITZERLAND ................................................ 121\n");
        printf("\n");


}
employee()
{       char uname2[20],pass3[20];
        char *uid="Admin",*psd="123";
        int len1,len2;

        printf("\nLogin for Company Employee");
        printf("\nEnter your Username:");
        scanf ("%s",&uname2);
        fflush(stdin);
        printf("Enter your Password:");
        scanf ("%s",&pass3);

        len1=strcmp(uid,uname2);
	len2=strcmp(psd,pass3);
        if(len1!=0 && len2!=0)
	    {
		    printf("YOU HAVE ENTERED WRONG USERNAME OR PASSWORD\n");
                    employee();
	    }
	    else
	    {
		    
	    }
}

void main()

{   
    int choice2,mob[10],dob[10];
        char pass[20],fname[20],lname[20],mail[30],pass2[20],sub[1];
        


    printf("\n");
    printf("                                    Increase the Adoption of Technologies by Farmers to Get Higher Production                                                ");
    printf("\n                                                            Creator: Kathan Desai                                                                            ");
int choice1;
printf("\n");
printf("\n<=================================================================================================================================================>");
printf("\n                        Press <1> for Farmer's / General Public Login:                                                      ");
printf("\n                        Press <2> for Company Employee Login:                                                               ");
printf("\n                        Press <3> to Exit:                                                                                  ");
printf("\n<================================================================================================================================================>");
printf("\n                        Enter Login choice:");

scanf("%d",&choice1);

switch (choice1)

{

case 1: printf("Select option to Login / Signup for Farmer's / General Public:");
        printf("\nPress <1> to Farmer's / General Public Login:");
        printf("\nPress <2> for Farmer's / General Public Signup:");
        printf("\nSelect for Login or Signup:");
        
        
        scanf("%d",&choice2);
        switch (choice2)
        {
            case 1: farmer_login();
                    content();
                    
            break;

            case 2: printf("Enter your First Name:");
                    scanf ("%s",&fname);
                    fflush(stdin);
                    printf("\nEnter your Last Name:");
                    scanf ("%s",&lname);
                    fflush(stdin);
                    printf("\nEnter your Mail Id:");
                    scanf ("%s",&mail);
                    fflush(stdin);
                    printf("\nEnter your Mobile Number:");
                    scanf ("%d",&mob);
                    fflush(stdin);
                    printf("\nEnter you2r Date of Birth:");
                    scanf ("%d",&dob);
                    fflush(stdin);
                    printf("\nEnter your Password for Login:");
                    scanf ("%s",&pass2);
                    fflush(stdin);
                    printf("\n<--------------------------------------------------------------------------------------->");
                    printf("\nType <Y> or <N> in SUBMIT to agree or disagree the Terms and Conditions:");
                    fflush(stdin);
                    
                    printf("\nSUBMIT:");
                    scanf("%s",&sub);
                    fflush(stdin);
                    
                    printf("<-------------------------------------Login Page------------------------------------>");
                    farmer_login();

                    content();
            break;                  
        }

        break;

case 2: 

	employee();
	
        break;

case 3 : exit(0);
}      
}  
