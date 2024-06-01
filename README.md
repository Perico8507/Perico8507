- 👋 Hi, I’m @Perico8507
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
Perico8507/Perico8507 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
using (HttpClient client = new HttpClient())
{
    try    
    {
        var response = await client.GetStreamAsync("https://smn.cna.gob.mx/webservices/?method=1");
    }  
    catch(HttpRequestException e)
    {
        Console.WriteLine("\nException Caught!");    
        Console.WriteLine("Message :{0} ",e.Message);
    }
}
