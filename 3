using System;
using System.Net.Http;
using System.Text.RegularExpressions;
using System.Threading.Tasks;

class Program
{
    static async Task Main()
    {
        string dotNetUrl = "https://en.wikipedia.org/wiki/.NET";

        using HttpClient client = new HttpClient();
        client.DefaultRequestHeaders.Add("User-Agent", "CSharpApp");

        string htmlDotNet = await client.GetStringAsync(dotNetUrl);

        // Знаходимо посилання, що, ймовірно, веде на semantic versioning
        var linkMatch = Regex.Match(htmlDotNet,
            @"<a [^>]*href\s*=\s*""(?<url>/wiki/[^""]*semantic[^""]*)""",
            RegexOptions.IgnoreCase);
        if (!linkMatch.Success)
        {
            Console.WriteLine("Link to semantic versioning not found.");
            return;
        }

        string relUrl = linkMatch.Groups["url"].Value;
        string fullUrl = "https://en.wikipedia.org" + relUrl;
        Console.WriteLine("Found link: " + fullUrl);

        string htmlSem = await client.GetStringAsync(fullUrl);

        // Витягуємо секцію “History” — від “== History ==” до наступного розділу “==”
        var historyMatch = Regex.Match(htmlSem,
            @"==\s*History\s*==(?<content>[\s\S]*?)(?==\s*[A-Za-z])",
            RegexOptions.IgnoreCase);
        if (historyMatch.Success)
        {
            string historyText = historyMatch.Groups["content"].Value.Trim();
            Console.WriteLine("History section content:");
            Console.WriteLine(historyText);
        }
        else
        {
            Console.WriteLine("History section not found.");
        }
    }
}
