using System;

namespace PasswordChecker
{
  class Program
  {
    public static void Main(string[] args)
    {

      int minLength = 9;
      string uppercase = "ABCDEFGHIJKLMNÑOPQRSTUVWYZ";
      string lowercase = "abcdefghijklmnñopqrstuvwxyz";
      string digits = "0123456789";
      string specialChars = "+-?!$@#*";

Console.Write("Please, introduce a password: ");
string password = Console.ReadLine();
int score = 0;

if (password.Length >= minLength)
{
  score++;
}

if (Tools.Contains(password, uppercase))
{
  score++;
}

if (Tools.Contains(password, lowercase))
{
  score++;
}
if (Tools.Contains(password, digits))
{
  score++;
}

if (Tools.Contains(password, specialChars))
{
  score++;
}

if (Tools.Contains(password, "password"))
{
  score = 0;
}
if(Tools.Contains(password, "1234"))
{
  score = 0;
}

Console.WriteLine(score);
switch (score)
{
  case 1:
  Console.WriteLine("The password is weak");
  break;
  case 2:
  Console.WriteLine("The password is medium");
  break;
  case 3:
  Console.WriteLine("The password is strong");
  break;
  case 4:
  case 5:
  Console.WriteLine("The password is super strong");
  break;
  default:
  Console.WriteLine("The password doesnt meet any of the standards");
  break;

}
    }
  }
}
