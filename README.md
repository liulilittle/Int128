# In128
Implement int128 bit integer various operators
 
Sample
----------------------
Ns::Int128 a = 0xf;
<br/>
Ns::Int128 b = a * 17;
<br/>
Ns::Int128 c = (b + 1) / a;
<br/>
Ns::Int128 d = (b + 1) % a;
<br/>
<br/>
std::strstream ss;
<br/>
ss &lt;&lt; a;
<br/>
Ns::Int128 lo;
<br/>
ss &gt;&gt; lo;
<br/>
<br/>
    printf("DEC: %s\nHEX: %s\nBIN: %s\n",<br/>
        (a << 100).ToString().data(), <br/>
        (a << 100).ToHex().data(),<br/>
        (a << 100).ToBinary().data());<br/>
<br/>
    printf("DEC: %s\nHEX: %s\nBIN: %s\n",<br/>
        ((a << 100) >> 97).ToString().data(),<br/>
        ((a << 100) >> 97).ToHex().data(),<br/>
        ((a << 100) >> 97).ToBinary().data());<br/>
<br/>
    printf("DEC: %s\nHEX: %s\nBIN: %s\n",<br/>
        (a--).ToString().data(),<br/>
        (a).ToHex().data(),<br/>
        (--a).ToBinary().data());<br/>
<br/>
    printf("DEC: %s\nHEX: %s\nBIN: %s\n",<br/>
        (a).ToString().data(),<br/>
        (a).ToHex().data(),<br/>
        (a).ToBinary().data());<br/>
<br/>
