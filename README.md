# Hello, there! 👋🏻

```typescript
/**
 * DeveloperSkillsInterface defines categorized skills
 * for Frontend, Backend, and Mobile development.
 */
interface DeveloperSkillsInterface {
  /** Frontend development skills */
  frontend: string[];

  /** Backend development skills */
  backend: string[];

  /** Mobile development skills */
  mobile: string[];
}

/**
 * Function to display developer skills by category.
 * @param skills - DeveloperSkillsInterface instance.
 * @returns A formatted string of skills grouped by category.
 */
const showSkills = (skills: DeveloperSkillsInterface): string => {
  return Object.entries(skills)
    .map(([category, values]) => {
      return `${category.toUpperCase()}:\n${values.map(v => `✔ ${v}`).join("\n")}`;
    })
    .join("\n\n");
};

// Example usage
const jesusSkills: DeveloperSkillsInterface = {
  frontend: ["TypeScript", "React", "HTML5", "CSS3", "Webpack"],
  backend: ["Node.js", "Express", "REST APIs", "Database Design"],
  mobile: ["React Native", "Expo", "Cross-platform Development"],
};

console.log(showSkills(jesusSkills));
```

> FRONTEND:  
> ✔ TypeScript  
> ✔ React  
> ✔ HTML5  
> ✔ CSS3  
> ✔ Webpack  

> BACKEND:  
> ✔ Node.js  
> ✔ Express  
> ✔ REST APIs  
> ✔ Database Design  

> MOBILE:  
> ✔ React Native  
> ✔ Expo  
> ✔ Cross-platform Development

##

> Built with '\u{2665}' (♥) by Jesús Domínguez [@jdomingu19](https://github.com/jdomingu19/)
