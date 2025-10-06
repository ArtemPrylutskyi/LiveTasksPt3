using System;
using System.Net.Http;
using System.Text.RegularExpressions;
using System.Threading.Tasks;

class Program
{
    static async Task Main()
    {
        string url = "https://learn.microsoft.com/en-us/dotnet/csharp/tour-of-csharp/overview";

        using HttpClient client = new HttpClient();
        string html = await client.GetStringAsync(url);

        string text = Regex.Replace(html, "<.*?>", " ");

        var sentenceMatch = Regex.Match(text, @"[^.?!]*\basync and await\b[^.?!]*[.?!]", RegexOptions.IgnoreCase);
        Console.WriteLine("1.1) Sentence with 'async and await':");
        Console.WriteLine(sentenceMatch.Success ? sentenceMatch.Value.Trim() : "Not found.");
        Console.WriteLine();

        var paragraphMatch = Regex.Match(text, @"([^\n]*equivalent format[^\n]*)", RegexOptions.IgnoreCase);
        Console.WriteLine("1.2) Paragraph with 'equivalent format':");
        Console.WriteLine(paragraphMatch.Success ? paragraphMatch.Value.Trim() : "Not found.");
        Console.WriteLine();

        int programCount = Regex.Matches(text, @"\b\w*program\w*\b", RegexOptions.IgnoreCase).Count;
        Console.WriteLine($"1.3) Count of words with 'program': {programCount}");
    }
}
