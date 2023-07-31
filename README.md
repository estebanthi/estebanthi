```batch
npx estebanthi-introduce
```

Hi👋, I'm **Esteban Thilliez** and I'm a **Student/Self-Employed**, based in **Lille, FR**📍.

I love working with **JavaScript** and **Python** using **Next.js, React, Vue, Node.js** and **Django, Flask**. I also know **Java** and **C**.

I'm interested in **Open source, AI, Data**, and **Algorithmic Trading**.

I like music 🎵 (I play **Piano and Guitar**), sport 🏃 (especially **Running and Bodybuilding and MMA**), piloting ✈️, reading 📖 (I read **52 books a year**), writing 🖊️ (**Blogging and Literature**), and trading 💹 (*And eventually losing money 😅*).

📬: You can contact me via [email](mailto:contact@esteban-thilliez.com), [LinkedIn](https://www.linkedin.com/in/esteban-thilliez-a210a5207/), or on [my website](https://www.esteban-thilliez.com).

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
    trading: "And eventually losing money 😅"
    },
    contact: {
        email: "mailto:contact@esteban-thilliez.com",
        linkedin: "https://www.linkedin.com/in/esteban-thilliez-a210a5207/",
        website: "https://www.esteban-thilliez.com",
    },

    introduce: function() {
        const introduction = `Hi👋, I'm **${this.name}** and I'm a **${this.occupation}**, based in **${this.location}**📍.`;
        const languages = `I love working with **${this.languages.javascript[0]}** and **${this.languages.python[0]}** using **${this.languages.javascript[1].join(", ")}** and **${this.languages.python[1].join(", ")}**. I also know **${this.languages.java[0]}** and **${this.languages.c[0]}**.`;
        const interests = `I'm interested in **${this.interests.slice(0, -1).join(", ")}**, and **${this.interests.slice(-1)}**.`;
        const hobbies = `I like music 🎵 (I play **${this.hobbies.music.join(" and ")}**), sport 🏃 (especially **${this.hobbies.sport.join(" and ")}**), piloting ✈️, reading 📖 (I read**${this.hobbies.reading}**), writing 🖊️ (**${this.hobbies.writing.join(" and ")}**), and trading 💹 (*${this.hobbies.trading}*).`;
        const contact = `📬: You can contact me via [email](${this.contact.email}), [LinkedIn](${this.contact.linkedin}) or on [my website](${this.contact.website}).`;
        const hello = `${introduction}\n\n${languages}\n\n${interests}\n\n${hobbies}\n\n${contact}`;

        const stats = this.generateStats();

        const message = `${hello}\n\n${stats}`;
        console.log(message);
    }
    generateStats: function() {
      return "## Some stats\n" +
          "![estebanthi's Stats](https://github-readme-stats.vercel.app/api?username=estebanthi&theme=vue-dark&show_icons=true&hide_border=true&count_private=true)"
    },
};

estebanthi.introduce()
estebanthi.generateStats()
```
