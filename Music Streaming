// C++ program to calculate the total earnings on the song based on the payment rates for the streaming service chosen.
#include <iostream>
#include <iomanip>
using namespace std;

// define the constants for the charges in each streaming service
#define TIDAL 0.01250
#define Amazon 0.00402
#define Apple_Music 0.00735
#define Spotify 0.00437
#define YouTube 0.00069

int main() {

   int choice;
   string artist, song;
   int streams;
   double earnings;
   string streamingService;

   // input of streaming service choice
   cout<<"Which Streaming Service will you use to upload your song? "<<endl;
   cout<<"\t1: TIDAL"<<endl;
   cout<<"\t2: Amazon"<<endl;
   cout<<"\t3: Apple Music"<<endl;
   cout<<"\t4: Spotify"<<endl;
   cout<<"\t5: Youtube"<<endl;
   cout<<"\nEnter your choice(1-5) : ";
   cin>>choice;

   // validate the choice
   if(choice < 1 || choice > 5)
   {
       cout<<endl<<"ERROR - NOT A VALID STREAMING SERVICE. PROGRAM WILL TERMINATE"<<endl;
   }else
   {
       // input of artist name, song name
       cin.ignore(100,'\n');
       cout<<endl<<"What is the artist's name? ";
       getline(cin,artist);
       artist = artist.substr(0,artist.length()-1); // remove '\n' from end
       cout<<endl<<"What is the name of the song? ";
       getline(cin,song);
       song = song.substr(0,song.length()-1); //remove '\n' from end

       // based on the streaming choice input the number of streams and calculate the total earnings if number of streams is positive
       // if number of streams is negative then print error and terminate
       if(choice == 1)
       {
           streamingService = "TIDAL";
           cout<<endl<<"How many streams does "<<song<<" have on TIDAL ? ";
           cin>>streams;

           if(streams < 0)
           {
               cout<<endl<<"ERROR - NUMBER OF STREAMS CANNOT BE NEGATIVE. PROGRAM WILL TERMINATE"<<endl;
               return 1;
           }else
           {
               earnings = streams*TIDAL;
           }
       }else if(choice == 2)
       {
           streamingService = "Amazon";
           cout<<endl<<"How many streams does "<<song<<" have on Amazon ? ";
           cin>>streams;

           if(streams < 0)
           {
               cout<<endl<<"ERROR - NUMBER OF STREAMS CANNOT BE NEGATIVE. PROGRAM WILL TERMINATE"<<endl;
               return 1;
           }else
           {
               earnings = streams*Amazon;
           }
       }else if(choice == 3)
       {
           streamingService = "Apple Music";
           cout<<endl<<"How many streams does "<<song<<" have on Apple Music ? ";
           cin>>streams;

           if(streams < 0)
           {
               cout<<endl<<"ERROR - NUMBER OF STREAMS CANNOT BE NEGATIVE. PROGRAM WILL TERMINATE"<<endl;
               return 1;
           }else
           {
               earnings = streams*Apple_Music;
           }
       }else if(choice == 4)
       {
           streamingService = "Spotify";
           cout<<endl<<"How many streams does "<<song<<" have on Spotify ? ";
           cin>>streams;

           if(streams < 0)
           {
               cout<<endl<<"ERROR - NUMBER OF STREAMS CANNOT BE NEGATIVE. PROGRAM WILL TERMINATE"<<endl;
               return 1;
           }else
           {
               earnings = streams*Spotify;
           }
       }else
       {
           streamingService = "YouTube";
           cout<<endl<<"How many streams does "<<song<<" have on YouTube ? ";
           cin>>streams;

           if(streams < 0)
           {
               cout<<endl<<"ERROR - NUMBER OF STREAMS CANNOT BE NEGATIVE. PROGRAM WILL TERMINATE"<<endl;
               return 1;
           }else
           {
               earnings = streams*YouTube;
           }
       }

       // if all valid values print the result
       cout<<endl<<"Song Name : "<<song<<endl;
       cout<<"Artist Name : "<<artist<<endl;
       cout<<"Streaming Service : "<<streamingService<<endl;
       cout<<"Streams : "<<streams<<endl;
       cout<<fixed<<setprecision(2)<<"Earnings : $"<<earnings<<endl;
   }
   return 0;
}
//end of program
