```batch
npx estebanthi-introduce
```

Hið, I'm **Esteban Thilliez** and I'm a **Student/Self-Employed**, based in **Lille, FR**ð.

I love working with **JavaScript** and **Python** using **Next.js, React, Vue, Node.js** and **Django, Flask**. I also know **Java** and **C**.

I'm interested in **Open source, AI, Data**, and **Algorithmic Trading**.

I like music ðµ (I play **Piano and Guitar**), sport ð (especially **Running and Bodybuilding and MMA**), piloting âï¸, reading ð (I read **52 books a year**), writing ðï¸ (**Blogging and Literature**), and trading ð¹ (*And eventually losing money ð*).

ð¬: You can contact me via [email](mailto:esteban.thilliez@gmail.com), [LinkedIn](https://www.linkedin.com/in/esteban-thilliez-a210a5207/), [GitHub](https://github.com/estebanthi), or [Medium](https://medium.com/@estebanthi).

## Some stats
![estebanthi's Stats](https://github-readme-stats.vercel.app/api?username=estebanthi&theme=vue-dark&show_icons=true&hide_border=true&count_private=true)

## Source
```javascript
const estebanthi = {
  name: "Esteban Thilliez",
  pronouns: ["he", "him"],
  location: "Lille, FR",
  occupation: "Student/Self-Employed",
  languages: {
    javascript: ["JavaScript", ["Next.js", "React", "Vue", "Node.js"]],
    python: ["Python", ["Django", "Flask"]],
    java: ["Java"],
    c: ["C"]
  },
  interests: ["Open source", "AI", "Data", "Algorithmic Trading"],
  hobbies: {
    music: ["Piano", "Guitar"],
    sport: ["Running", "Bodybuilding", "MMA"],
    piloting: "Private Pilot License",
    reading: "52 books a year",
    writing: ["Blogging", "Literature"],
    trading: "And eventually losing money ð"
    },
    contact: {
        email: "mailto:esteban.thilliez@gmail.com",
        linkedin: "https://www.linkedin.com/in/esteban-thilliez-a210a5207/",
        github: "https://github.com/estebanthi",
        medium: "https://medium.com/@estebanthi",
    },
    generateStats: function() {
      return "## Some stats\n" +
          "![estebanthi's Stats](https://github-readme-stats.vercel.app/api?username=estebanthi&theme=vue-dark&show_icons=true&hide_border=true&count_private=true)"
    },
    introduce: function() {
        const introduction = `Hið, I'm **${this.name}** and I'm a **${this.occupation}**, based in **${this.location}**ð.`;
        const languages = `I love working with **${this.languages.javascript[0]}** and **${this.languages.python[0]}** using **${this.languages.javascript[1].join(", ")}** and **${this.languages.python[1].join(", ")}**. I also know **${this.languages.java[0]}** and **${this.languages.c[0]}**.`;
        const interests = `I'm interested in **${this.interests.slice(0, -1).join(", ")}**, and **${this.interests.slice(-1)}**.`;
        const hobbies = `I like music ðµ (I play **${this.hobbies.music.join(" and ")}**), sport ð (especially **${this.hobbies.sport.join(" and ")}**), piloting âï¸, reading ð (I read**${this.hobbies.reading}**), writing ðï¸ (**${this.hobbies.writing.join(" and ")}**), and trading ð¹ (*${this.hobbies.trading}*).`;
        const contact = `ð¬: You can contact me via [email](${this.contact.email}), [LinkedIn](${this.contact.linkedin}), [GitHub](${this.contact.github}), or [Medium](${this.contact.medium}).`;
        const hello = `${introduction}\n\n${languages}\n\n${interests}\n\n${hobbies}\n\n${contact}`;

        const stats = this.generateStats();

        const message = `${hello}\n\n${stats}`;
        console.log(message);
    }
};

estebanthi.introduce()
```