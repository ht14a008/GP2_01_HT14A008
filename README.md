# GP2_01_HT14A008
GP2_01_HT14A008

#include <iostream>#define GP2_PRIME_UPPER_LIMIT  1000000
int nth_prime(unsigned int a,unsigned int b,unsigned int n){ int number = 0; for(int j = 0;j < GP2_PRIME_UPPER_LIMIT;j++){  if(a == 2){   number++;  }    if(a > 2){   int chk = a;   int jag = 0;   for(int l = 3;l < chk;l++){    if(chk % l == 0){     l = a;     jag = 1;    }   }   if(jag == 0){    number++;   }  }
  if(number == n){   break;  }  a = a + b; } return a;}
int main(){ std::cout << nth_prime(367,186,151) << std::endl; std::cout << nth_prime(179,10,203) << std::endl; std::cout << nth_prime(271,37,39) << std::endl; std::cout << nth_prime(103,230,1) << std::endl; std::cout << nth_prime(27,104,185) << std::endl; std::cout << nth_prime(253,50,85) << std::endl; std::cout << nth_prime(1,1,1) << std::endl; std::cout << nth_prime(9075,337,210) << std::endl; std::cout << nth_prime(307,24,79) << std::endl; std::cout << nth_prime(331,221,177) << std::endl; std::cout << nth_prime(259,170,40) << std::endl; std::cout << nth_prime(269,58,102) << std::endl; std::cin.get(); return 0;}
