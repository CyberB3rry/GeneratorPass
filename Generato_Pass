/*
    PASSWORD GENERATOR
*/
#include<iostream>
#include<cstdlib>
using namespace std;

char alpha[27] = {'a','b','c','d','e','f','g','h','i','j','k','l','m','n','o','p','q','r','s','t','u','v','w','x','y','z'};
char Alpha[27] = {'A','B','C','D','E','F','G','H','I','J','K','L','M','N','O','P','Q','R','S','T','U','V','W','X','Y','Z'};
char number[10] = {'1','2','3','4','5','6','7','8','9','0'};
char special[7] = {'(',')','!','"','@','/','='};

int main()
{
    char password[100];
    int ran, ran1, choice, lenght;

    do
    {
        cout<<"Choose the length of the characters: ";
        cin>>lenght;
        
        srand(time(NULL));
        for(int i=0; i<lenght; i++)
        {
            ran = rand()%4;
            if(ran == 0) //MINUSCOLO
            {
                ran1 = rand()%27;
                password[i] = alpha[ran1];
            }else if(ran == 1) //MAIUSCOLO
            {
                ran1 = rand()%27;
                password[i] = Alpha[ran1];
            }else if(ran == 2) //NUMERI
            {
                ran1 = rand()%10;
                password[i] = number[ran1];
            }else if(ran == 3) //SPECIALI
            {
                ran1 = rand()%7;
                password[i] = special[ran1];
            }
        }
        
        cout<<"\n";
        cout<<"Password: ";
        for(int j=0; j<lenght; j++)
            cout<<password[j];
        cout<<"\n";
        cout<<"\nDo you want to continue? [Y=1 N=0]: ";
        cin>>choice;
    }while(choice != 0);
    return 0;
}
