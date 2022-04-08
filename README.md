# prime-numbers
finding the prime number
var n=88;
var end=n;
var store="";
for(var i=2; i<=n; i=i)
  {
if (n%i==0)
    { 
      var present=false;
      for (var j=2; j<=Math.sqrt(i); j++)
        {
          if (i%j==0)
          {
            present=true;
            break;
          }
        }
      
     if (present==false)
     {
       store+=i+" ";
     }
     n=n/i;
    }
else 
{
  i++;
}
  }
console.log(store);
