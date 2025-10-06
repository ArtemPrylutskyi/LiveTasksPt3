using System;
using System.Net.Http;
using System.Text.RegularExpressions;
using System.Threading.Tasks;

class Program
{
    static async Task Main()
    {
        string url = "https://unsplash.com/wallpapers";

        using HttpClient client = new HttpClient();
        client.DefaultRequestHeaders.Add("User-Agent", "CSharpApp"); 

        try
        {
            string html = await client.GetStringAsync(url);

            var matches = Regex.Matches(html, @"https://images\.unsplash\.com/[^\s""']+\.(jpg|jpeg|png)");

            Console.WriteLine($" Found {matches.Count} image links:");
         

            int i = 1;
            foreach (Match match in matches)
            {
                Console.WriteLine($"{i++}. {match.Value}");
            }
        }
        catch (Exception ex)
        {
            Console.WriteLine(" Error fetching images:");
            Console.WriteLine(ex.Message);
        }
    }
}

