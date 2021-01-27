### About Me
For more information, please visit [my website](https://www.jo3-w3b-d3v.com/). 🙂

```html
<!-- This section covers a bit about me. -->
<!-- AKA. The boring part 😴 ... -->
<p>
    I’m a young, ambitious & highly driven nerd, aiming <br/>
    to go far within the world of software engineering. I <br/>
    typically enjoy working with microservice or SOA architectures <br/>
    & I enjoy working across the entire stack. <br/>
    You could say that I'm a bilingual software engineer.
</p>

<b>I am always eager to learn more. 🎓</b>
```

```javascript
// Return a list of tech that I'm passioante about. 
const myFavouriteTech = () => {
    return [
        "Java",
        "JavaScript",
        "Python",
        "PHP",
        "Kubernetes",
        "Docker",
        "SQL",
        "Cloud Technologies", //GCP, Azure, AWS, etc.
        "Progressive Web Applications" // HTML, CSS, etc.
    ];
};

console.log(myFavouriteTech());
```

```java
public class Inspiration {

    // Return a list of nerds that really inspire me.
    public ArrayList<Nerd> getInspiration() {
        ArrayList<Nerd> nerds = new ArrayList<>();
        nerds.add(Nerd.builder().name("Martin Fowler").url("https://martinfowler.com/").build());
        nerds.add(Nerd.builder().name("Eric Elliott").url("https://ericelliottjs.com/").build());
        nerds.add(Nerd.builder().name("Krasimir Tsonev").url("https://krasimirtsonev.com/").build());
        nerds.add(Nerd.builder().name("Raymond Camden").url("https://www.raymondcamden.com/").build());
        nerds.add(Nerd.builder().name("Stefan Mischook").url("https://www.killersites.com/about/").build());
        nerds.add(Nerd.builder().name("Darcey Lloyd").url("https://aftc.io/").build());
        return nerds;
    }
}
```

```python
class JO3W3BD3V:
    def __init__(self):
        self.shortTermGoals = []
        
        self.shortTermGoals.append("Learn more about machine learning.")
        self.shortTermGoals.append("Learn more about big data.")
        self.shortTermGoals.append("Try to master RDBMS.")

        # Touch wood 
        self.shortTermGoals.append("Get some freelance projects on the side.")
    
    def getShortTermGoals(self):
        return self.shortTermGoals
                
me = JO3W3BD3V()
print(me.getShortTermGoals())
```

```SQL 
DROP TABLE IF EXISTS Experiences;

CREATE TABLE Experiences(
    id INT AUTO_INCREMENT NOT NULL,
    title VARCHAR(50) NOT NULL,
    company VARCHAR(75) NOT NULL,
    startDate VARCHAR(7) NOT NULL,
    endDate VARCHAR(7),
    description VARCHAR(250) NOT NULL,
    PRIMARY KEY(id)
);

CREATE INDEX ExperiencesTitleIndx ON Experiences(title);
CREATE INDEX ExperiencesCompanyIndx ON Experiences(company);
CREATE INDEX ExperiencesStartDateIndx ON Experiences(startDate) USING BTREE;
CREATE INDEX ExperiencesEndDateIndx ON Experiences(endDate) USING BTREE;

INSERT INTO Experiences(title, company, startDate, endDate, description)
VALUES('Software Engineer', 'Lloyds Bank', '05/2020', NULL, 'I currently work in motor finance, where I currently use technologies including C#, Java, Angular, Jenkins, etc.'),
    ('Software Engineer', 'Admiral', '03/2019', '05/2020', 'I worked on the van insurance product(s), I used technologies like K8s, Azure, Azure DevOps, Docker, Angular & Java.'),
    ('Software Developer', 'Inngot', '05/2018', '03/2019', 'I worked mostly as a front end developer, using react, I would sometimes use Java for the back end.'),
    ('Web Developer', 'Cruise Nation', '12/2017', '05/2018', 'I worked as a front end developer, ensuring that the customer experience was my number one priroity.'),
    ('Juniour Web Developer', 'BVG', '02/2017', '12/2017', 'I worked as a full stack developer, though I mostly focused on implemengint pretty admin consoles, funky AJAX tools & increasing the performance of database queries.');
    
-- Get all of my past experiences.
SELECT * FROM Experiences;
```
