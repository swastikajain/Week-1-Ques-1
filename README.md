1.
#include <iostream>
using namespace std ;
void search(int *a,int n ,int key){
    int count = 0 ;
        for(int i=0;i<n;i++){
            count++;
            if(a[i] == key){
                cout<<"Element found at index : "<<i<<endl;
                break;
            }
                
                
        }
        cout<<"Total comparisons : "<<count;

}
void insert(int *a,int n){
    for(int i=0;i<n;i++)
        cin>>a[i];
}
int main(){
    int n ;
    cout<<"Enter the size of array : "<<endl ; 
    cin>>n;
    int *a = new int[n] ;
    cout<<"Enter "<<n<<" elements : "<<endl ;
    insert(a ,n );
    int key ;
    cout<<"Enter the element to search :"<<endl;
    cin>>key;
    search(a,n,key);
    
}
