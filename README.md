# Oi, eu sou o Tallys 👋

```csharp
public class Developer
{
    public string Name { get; set; } = "Desenvolvedor .NET";
    public int ExperienceYears { get; set; } = Datetime.Now.Year - 2006;
    public string[] Expertise { get; set; } = { "Setor Financeiro", "Bancário", "Seguradoras", "BPO" };
    public string Focus { get; set; } = "Cibersegurança";
    public string ProudTitle { get; set; } = "Pai do Gustavo";
    public string Mission { get; set; } = "Explorando novos desafios e criando um futuro digital mais seguro!";
    
    public void BuildCareer()
    {
        Console.WriteLine("Transformando o futuro com experiência e segurança.");
    }

    public void ReadReadmeTitle(bool usingGokuVoice)
    {
        ValidationException.When(!usingGokuVoice, "Leia novamente o título deste README ultilizando a voz do Goku :)");
    }
}

public class ValidationException : Exception
{
    public ValidationException(string error) : base(error)
    { }

    public static void When(bool hasError, string errorMessage)
    {
        if (hasError)
            throw new ValidationException(errorMessage);
    }
}
