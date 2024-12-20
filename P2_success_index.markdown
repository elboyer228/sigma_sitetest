---
layout: page 
title: Success index 
permalink: /success/
---

## Movie success index 
### Finding relevent features 
In order to assess and define actors' careers, they first had to answer a crucial question: **“What makes a movie truly successful?”**

Over a beer at a local bar, they were debating the question:

> **“Profit!”** shouted Mathieu, who had dreamed of becoming a millionaire star since he was three years old.  
>
> **“No way, it’s about revenue,”** countered Mael, who’d seen *Avengers* too many times to think otherwise.  
>
> **“Reviews!”** argued Aiden.  “If IMDb doesn’t like it, I don’t like it.”  
>
> **“Oscars matter, though,”** whispered Elise, as Pol nodded solemnly. “Nobody argues with gold statues.”

To settle the debate, the friends decided to design the **Movie Success Index**—a system to rank movies based on **profitability**, **revenue**, **reviews**, and **Oscar nominations**.

Since they had been paying close attention during their ADA lectures, they knew that the data needed some transformation to make it both meaningful and usable.

- For the **profitability factor**, Mathieu used the data on revenue and budget to calculate the ratio. However, even though Mathieu’s eyes sparkled at the sight of massive revenue numbers, he knew that to scale everything correctly from 0 to 10, he had to apply a log transformation. This smoothed out the extreme values caused by colossal blockbusters.
<div style="text-align: center;overflow: hidden;">
<iframe 
        src="{{ '/assets/plots/responsive_graph.html' | relative_url }}" 
        width="900px" 
        height="400px" 
        frameborder="0"
        style="overflow: hidden; border: none;">
</iframe>
</div>

- For the **revenue factor**, Mael took charge:  
  *“Box office revenue is massive, but we log-transformed it too. Otherwise, Avatar would crush everything forever. This way, even low-budget hits look respectable.”*

<div style="text-align: center;overflow: hidden;">
<iframe 
        src="{{ '/assets/plots/movie_revenue_distribution.html' | relative_url }}" 
        width="900px" 
        height="400px" 
        frameborder="0"
        style="overflow: hidden; border: none;">
</iframe>
</div>

Now, both profitability and revenue were neatly scaled from 0 to 10.



- Aiden, the IMDb enthusiast, happily handled the **reviews factor**, as ratings were already graded from 0 to 10.  
  *“Done and dusted. What a day!”* he exclaimed.

<div style="text-align: center; overflow: hidden;">
    <iframe 
        src="{{ '/assets/plots/movie_score_distribution.html' | relative_url }}" 
        width="900px" 
        height="300px" 
        frameborder="0" 
        style="overflow: hidden; border: none;">
    </iframe>
</div>


<style>
  .two-columns {
    display: flex; /* Use flexbox to create two columns */
    gap: 20px; /* Add spacing between columns */
    align-items: center; /* Align items vertically */
    justify-content: space-between; /* Space between text and image */
  }

  .text-column {
    flex: 1; /* Allocate space for text */
    font-size: 16px;
    line-height: 1.6;
  }

  .image-column {
    flex: 1; /* Allocate space for the image */
    text-align: center; /* Center the image */
  }

  img {
    max-width: 100%; /* Ensure image scales properly */
    height: auto; /* Maintain aspect ratio */
    border-radius: 5px; /* Optional: Rounded corners */
  }

  @media (max-width: 768px) {
    .two-columns {
      flex-direction: column; /* Stack content vertically on smaller screens */
    }
  }
</style>

<div class="two-columns">
  <!-- Text Column -->
  <div class="text-column">
    <p>
      Finally, Pol and Elise tackled the <strong>oscar nomination factor</strong>. Since a movie with many nominations already speaks for itself, they applied a log scale to ensure that each additional nomination added less weight. This way, the Oscars boosted the index without overwhelming it.
    </p>
  </div>

  <!-- Image Column -->
  <div class="image-column">
    <div style="overflow: hidden; transform: scale(0.8); width: 100%; height: 100%; display: flex; align-items: center;">
      <iframe 
          src="{{ '/assets/plots/oscar_nomination_distribution.html' | relative_url }}" 
          width="650px" 
          height="650px" 
          frameborder="0" 
          style="overflow: hidden;border: none;">
      </iframe>
    </div>
  </div>
</div>





### Crafting the Success Index

With their features defined, the group focused on combining them into a single score that could rank movies effectively. After thoughtful discussion, they assigned the following weights to capture the essence of a movie's success:

- **Popularity** (IMDb scores): 40%  
- **Profitability** (revenue-to-budget ratio): 15%  
- **Revenue**: 45%  

When it came to the **Oscar nomination factor**, Pol and Elise led the effort. They applied a logarithmic scale, ensuring that each additional nomination added diminishing weight. This approach kept the multiplier balanced while giving a fair edge to Oscar-nominated films.

Finally, the group normalized the combined scores so that the **Success Index** ranged from 0 to 10, allowing easy comparison across all movies.

From this analysis, they identified the **Top 5 Best Movies** and **Top 5 Worst Movies** based on the Success Index:


### **Top 5 Best Movies**

| Rank | Movie                                         | Year | Popularity | Revenue/Budget Ratio | Revenue Score | Success Index |
|------|-----------------------------------------------|------|------------|-----------------------|---------------|---------------|
| 1    | The Lord of the Rings: The Return of the King | 2003 | 7.92       | 8.9                   | 9.26          | 6.00          |
| 2    | The Lord of the Rings: The Fellowship of the Ring | 2001 | 7.85       | 8.8                   | 9.05          | 5.84          |
| 3    | Forrest Gump                                  | 1994 | 7.84       | 8.8                   | 8.85          | 6.02          |
| 4    | E.T. the Extra-Terrestrial                    | 1982 | 7.82       | 7.8                   | 8.98          | 7.26          |
| 5    | Avatar                                        | 2009 | 7.73       | 7.8                   | 10.00         | 5.99          |



### **Top 5 Worst Movies**

| Rank | Movie                 | Year | Popularity | Revenue/Budget Ratio | Revenue Score | Success Index |
|------|-----------------------|------|------------|-----------------------|---------------|---------------|
| 1    | Deadfall              | 1993 | 1.03       | 4.0                   | 0.26          | 0.00          |
| 2    | Dangerous Game        | 1993 | 1.52       | 5.6                   | 0.47          | 0.17          |
| 3    | Wicked Stepmother     | 1989 | 1.74       | 4.3                   | 0.97          | 1.54          |
| 4    | The Specials          | 2000 | 1.77       | 5.8                   | 0.00          | 1.35          |
| 5    | Best Laid Plans       | 1999 | 1.78       | 6.1                   | 0.60          | 0.53          |

---

As the group reviewed the rankings, Aiden noticed several of his favorite movies in the **Top 5 Best Movies** list. Smiling smugly, he declared:  **“I knew I had good taste.”**  

This approach allowed the group to identify the movies that best captured the magic of cinematic success and those that fell short of the mark. With the Success Index in hand, they now had a fair and consistent way to rank Hollywood's finest and not-so-finest productions.


## Actor success index 

### Crafting the Actor Success Index

After defining what makes a movie successful, the group turned to a more ambitious question: **“How do we measure the success of an actor’s career?”** It wasn’t just about starring in a blockbuster or being part of an award-winning cast. The team wanted to capture something deeper: the consistency, quality, and impact of an actor’s body of work over time.

> **“We need to go beyond averages,”** Pol said. **“It’s about the journey, not just the destination.”**

- **The main character bonus**: The first step was recognizing the importance of leading roles.  
  **“Landing a lead role is a sign of trust and star power,”** Elise explained. To reflect this, they gave a **25% boost** to the scores of movies where an actor played the main character.

- **Multipliers and streaks**: The next challenge was to capture consistency. The group devised a **multiplier and streak system**, where an actor’s movie scores were influenced by how their previous performances measured up.  
  If a movie performed as well as or better than the last, the multiplier increased, rewarding consistency. But if the movie underperformed, the multiplier dropped, reflecting dips in quality.

- **The final grade**: With the cumulative multiplier applied to each movie score, the results were summed up and transformed using a logarithmic scale to reflect diminishing returns for starring in many movies. Finally, they normalized the scores to a 0–10 scale, making them comparable across all actors.  
  The **Actor Success Index** became a tool not just for ranking actors but for telling the story of their journey through Hollywood—a perfect complement to their work on the Movie Success Index.

Using this index, they identified the **Top 5 Best Actors** and **Top 5 Worst Actors**:


### **Top 5 Best Actors**

| Rank | Actor              | Cumulative Score | Normalized Score |
|------|--------------------|------------------|------------------|
| 1    | Denzel Washington  | 3.53             | 10.00           |
| 2    | Matt Damon         | 3.44             | 9.69            |
| 3    | Tom Hanks          | 3.27             | 9.15            |
| 4    | Frank Welker       | 3.25             | 9.08            |
| 5    | Eddie Murphy       | 3.21             | 8.92            |


### **Top 5 Worst Actors**

| Rank | Actor              | Cumulative Score | Normalized Score |
|------|--------------------|------------------|------------------|
| 1    | Stuart Nisbet      | 0.71             | 0.52            |
| 2    | Vladimir Dolinsky  | 0.71             | 0.52            |
| 3    | Evelyn Keyes       | 0.68             | 0.40            |
| 4    | James Dixon        | 0.68             | 0.40            |
| 5    | Peter Fonda        | 0.56             | 0.00            |



> Aiden was thrilled to see his favorite actors dominating the Top 5, grinning smugly as he exclaimed:  
>
> **'I told you I have great taste!'**
>
> Meanwhile, Mathieu couldn’t hide his unease, noticing two of his favorite actors in the worst list and quietly questioning his cinematic preferences...

### Next: [Unveiling the Path to Stardom – Insights on Becoming a Successful Actor]({{'/results/'| relative_url }})
