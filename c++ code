#include<iostream>
using namespace std;
int main(){
    int size;
    cin>>size;
    const int a = size;
    char array[a][a];
    int mi=0,mj=0,pi=0,pj=0;
    for(int i=0;i<a;i++)
            for(int j=0;j<a;j++)
            cin>>array[i][j];

    for(int i=0;i<a;i++){
            for(int j=0;j<a;j++){
                    if(array[i][j]=='m'){
                            mi=i;
                            mj=j;
                    }
                    if(array[i][j]=='p'){
                            pi=i;
                            pj=j;
                    }
            }
    }

    while(mj!=pj||mi!=pi){
            if(mi==pi){
                    if(mj<pj)
                    {
                        cout<<"RIGHT"<<endl;
                        mj++;
                    }
                    if(mj>pj)
                    {
                        cout<<"LEFT"<<endl;
                        mj--;
                    }
            }
            if(mj==pj){
                    if(mi<pi)
                    {
                        cout<<"DOWN"<<endl;
                        mi++;
                    }
                    if(mi>>pi)
                    {
                        cout<<"UP"<<endl;
                        mi--;
                    }
            }
            else{
                    if(mi<pi)
                    {
                        if(mj<pj)
                        {
                            cout<<"DOWN"<<endl;
                            mi++;
                            if(mi==pi||mj==pj)
                                continue;
                            cout<<"RIGHT"<<endl;
                            mj++;
                            if(mi==pi||mj==pj)
                                continue;
                        }
                        if(mj>pj)
                        {
                            cout<<"DOWN"<<endl;
                            mi++;
                            if(mi==pi||mj==pj)
                                continue;
                            cout<<"LEFT"<<endl;
                            mj--;
                            if(mi==pi||mj==pj)
                                continue;
                        }
                    }
                    if(mi>pi)
                    {
                        if(mj>pj)
                        {
                            cout<<"UP"<<endl;
                            mi--;
                            if(mi==pi||mj==pj)
                                continue;
                            cout<<"LEFT"<<endl;
                            mj--;
                            if(mi==pi||mj==pj)
                                continue;
                        }
                        if(mj<pj)
                        {
                            cout<<"UP"<<endl;
                            mi--;
                            if(mi==pi||mj==pj)
                                continue;
                            cout<<"RIGHT"<<endl;
                            mj++;
                            if(mi==pi||mj==pj)
                                continue;
                        }
                    }



            }

    }

    return 0;
}
