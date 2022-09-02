#include <iostream>
using namespace std;
int main(int argc, char** argv) {
	srand(time(NULL));
	while(true)
	{
		int n=0;
		bool win=false;
		int somay=1+rand()%100;
	
		cout<<"chuong trinh tro` choi doan so :> \n";
		while(true)
		{
			cout<<"moi nhap so ma` ban doan trong [1...100]: \n";
			int songuoi;
			cin>>songuoi;
			if(songuoi>somay)
			{
				cout<<"so cua ban lon hon dap an! \n";
			}
			else if(songuoi<somay)
			{
				cout<<"so cua ban nho hon dap an! \n";
			}
			else
			{
				cout<<"CHUC MUNG` BAN, BAN DA~ DOAN DUNG ROI`!!!\n"<<"dap an la`: "<<somay;
				win==true;
				break;
			}
			n++;
			cout<<"ban da nhap "<<n<<" lan! \n";
			if(n==7)
			break;		
		}
		if(win!=true)
		{
			cout<<"Game Over!\n"<<"Dap an la`: "<<somay<<endl;
		}
		cout<<"Do you want try it again?\n"<<"Enter your choice(y/n):";
			char c;
			cin>>c;
			if(c=='n')
			{
				cout<<"Goodbye!";
				break;
			}
    }
	return 0;
}
