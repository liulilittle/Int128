# In128
Implement int128 bit integer various operators
 
Sample
----------------------
Ns::Int128 a = 0xf;
Ns::Int128 b = a * 17;
Ns::Int128 c = (b + 1) / a;
Ns::Int128 d = (b + 1) % a;

std::strstream ss;
ss << a;

Ns::Int128 lo;
ss >> lo;
