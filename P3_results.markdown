---
layout: page
title: The final answer of how to be a successful actor !
permalink: /results/
---

The team—Pol, Mael, Elise, Aiden, and Mathieu—was nearing the end of their journey. They had cracked the Movie Success Index, but as they dove deeper into actor attributes, they uncovered fascinating trends in demographics, education, and career trajectories coming from they final data set. They were about to answer their final question.

**What are the key features for actor success ? Can we find anypattern or key insights that could help predict the success of actors ?**


# Demographics
## Does gender play a role in defining success for actors?



<div style="text-align: center;">
<iframe 
        src="{{ '/assets/plots/success_score_vs_gender.html' | relative_url }}" 
        width="100%" 
        height="600px" 
        frameborder="0">
</iframe>
</div>


The plot told a fascinating story:

- Male actors showed a broad spread, with some reaching sky-high scores near the maximum of 10.
- Female actors, while clustering more tightly around the middle, rarely dipped into the extremes.

These results led to a debate:

Pol, ever the strategist, furrowed his brow. **“It’s not just about the scores. It’s about the opportunities that lead to these scores. How many female actors get the chance to star in major franchises or Oscar-bait films? Those roles can skew the range for men.”**

Mathieu, the eternal optimist, leaned forward. **“But what about outliers? Look at those female actors who’ve cracked the top. That’s inspiring—proof that greatness is possible, even in a skewed system.”**

Aiden, the data purist, shook his head. **“Hold on. Let’s not jump to conclusions. Gender might influence trends, but we need to dig deeper. What about age, genre, or even awards? This plot is just the start.”**

Even though some questions remained, two main conclusions could be drawn:
> 1. **Male success is more volatile:** Male actors dominate the extremes, reflecting both the opportunities and challenges of a male-driven industry.
> 2. **Female success is steady:** While fewer women hit the very top, their consistent performance suggests a different but equally valuable path to success.

## The physical presence of success
<div style="text-align: center;">
<iframe 
        src="{{ '/assets/plots/height_vs_gender.html' | relative_url }}" 
        width="100%" 
        height="600px" 
        frameborder="0">
</iframe>
</div>

The height distribution plot told an interesting story about physical presence in movies:

- Male actors predominantly clustered between 1.7m and 1.9m, with a notable peak around 1.8m, suggesting a preference for taller male leads.
- Female actors, on the other hand, formed a narrower range between 1.6m and 1.7m, aligning with traditional ideals of femininity portrayed in the industry.


These observations sparked a lively discussion among the group:

**“Height clearly influences casting decisions.”** Mael said, pointing at the chart. **"Just think of the classic leading man—tall, commanding, larger-than-life. It’s no surprise we see this preference reflected here.”**

Pol raised an eyebrow. **“Sure, but let’s not forget the exceptions. Actors like Tom Cruise or Reese Witherspoon don’t fit these height trends but are among the most successful. Maybe charisma and skill can defy these norms.”**

From there it appears that height appears to align with traditional gender roles in Hollywood:
> 1. **For men** , height may signify dominance or strength, fitting the archetypal “hero” mold.
> 1. **For women**, there may be an unspoken preference for certain heights, reflecting societal expectations of femininity.
>
> But outliers in both groups challenge these norms, proving that talent, charisma, and opportunity can still redefine success.


Elise added, “But this is only part of the story. Height might matter, but what about age, skills and education? Let’s dig further.”

# Carreer Trajectory
## The journey of success through time

<div style="text-align: center;">
<iframe 
        src="{{ '/assets/plots/age_first_release_vs_score.html' | relative_url }}" 
        width="100%" 
        height="600px" 
        frameborder="0">
</iframe>
</div>


From this plot clear insights where here : 

- Female actors show a noticeable decline in success scores as age increases. While younger actresses (ages 20–30) exhibit a wide range of success, this variability diminishes with age. This could indicate that the industry places a premium on younger actresses, potentially limiting opportunities for older women.

Elise commented, **“This highlights the pressure on female actors to establish their careers early. Older actresses face a narrowing range of roles, which may reflect larger industry biases.”**

- Male actors achieve their highest success scores predominantly between the ages of 20 and 40. After 40, the success scores stabilize but rarely reach the peaks seen in younger years.

 Mael noted, **“It’s not surprising. This is the age range where actors are cast as leading men in action movies, dramas, and blockbusters.”**

But for both distribution, graphs also reveals some outliers—both male and female actors who started their careers later (even into their 50s or 60s) and still achieved notable success.
This emphasizes that while trends exist, individual talent and the right opportunities can overcome age-related barriers.

Mathieu observed, **“These outliers remind us that success isn’t bound by age—it’s about the right role at the right time.”**



# Actor Attributes
## Education’s role in shaping success

<div style="text-align: center;">
<iframe 
        src="{{ '/assets/plots/school_vs_score.html' | relative_url }}" 
        width="100%" 
        height="600px" 
        frameborder="0">
</iframe>
</div>

The violin plot comparing success scores across different specialized school types provides valuable insights into how education shapes an actor’s career:
- Specialized Drama Schools Lead the Way: Actors trained in specialized drama schools achieve the highest success scores, with a significant proportion scoring above 6. This highlights the impact of formal, drama-focused training on career success.
- Arts Schools Show a Narrow Range: Arts schools display a limited range of success scores, with most actors scoring below 7. This indicates fewer opportunities for exceptionally high success compared to other school types.
- Acting and Dance Schools Show Modest Results: Specialized acting schools exhibit a narrower distribution, with success scores clustering around the mid-range (4–5). Meanwhile, specialized dance schools have the smallest representation and generally lower success scores, reflecting their more niche focus.

> **Training matters:** Actors from specialized drama schools or top-ranked universities often achieve higher success scores, reflecting the value of formal training.  
> **Exceptions prove the rule:** Outliers from dance schools, arts schools, or lower-ranked universities show that unconventional paths can still lead to success.  
> **Diversity of opportunity:** The varied distributions emphasize the unpredictability of the film industry, where individual talent can outweigh traditional advantages.

## The influence of university rank on success

<div style="text-align: center;">
<iframe 
        src="{{ '/assets/plots/uni_rank_vs_score.html' | relative_url }}" 
        width="100%" 
        height="600px" 
        frameborder="0">
</iframe>
</div>

The scatterplot exploring the relationship between university rank and success score was designed to address the question: **“Does attending a prestigious school lead to a more direct path to success?”**

*Note that for actors that did not go to university or to an un ranked university, the rank assigned was 3000.*
From the actors who attended university, we observe a clear trend: success scores tend to decrease as university rank increases.
- **Actors with high success scores:** those with a high success index are more likely to have attended highly-ranked universities, reflecting the advantages of access to better training, resources, and connections.
- **Decreasing success with lower ranks:** the number of actors achieving high success scores diminishes as university rank decreases, highlighting the impact of educational prestige.
- **Exceptions to the rule:** despite this trend, several actors from mid-ranked universities achieved notable success, proving that success is still possible beyond prestige.

Mael, ever the realist, observed, :**“Prestige clearly opens doors, but it’s not the only path to success. Talent and timing matter just as much.”:**
Aiden nodded, adding, :**“It’s encouraging to see those from less prestigious universities succeed—it’s a reminder that hard work and opportunity can break through any barrier.”:**

This suggests that while attending a prestigious university provides a clear edge, individual talent, determination, and opportunities can still lead to success regardless of an actor’s alma mater.

<div style="text-align: center;">
<iframe 
        src="{{ '/assets/plots/rank_fixed_vs_score.html' | relative_url }}" 
        width="100%" 
        height="600px" 
        frameborder="0">
</iframe>
</div>

## US geographic perspective of success 

<div style="text-align: center;">
<iframe 
        src="{{ '/assets/plots/prev_state_vs_score.html' | relative_url }}" 
        width="100%" 
        height="600px" 
        frameborder="0">
</iframe>
</div>

<div style="text-align: center;">
<iframe 
        src="{{ '/assets/plots/state_vs_score.html' | relative_url }}" 
        width="100%" 
        height="600px" 
        frameborder="0">
</iframe>
</div>


The map told a fascinating story:  

- **Variability across states:** some states, particularly in the Midwest, show higher average success scores, while others in the South and West tend to score lower on average.  
- **Cluster of success:** a few standout states consistently achieve higher average scores, suggesting regional influences on success rates in Hollywood.  


These results led to a lively discussion among the group:  

Pol, ever the strategist, furrowed his brow. **“It’s not just about where actors are born—it’s about the opportunities available to them. Are these high-scoring states producing more actors, or are they just offering better early training and support?”**  

Mathieu, the eternal optimist, leaned forward. **“But what about states with lower scores? Maybe they’re underrepresented because they lack the infrastructure to support aspiring actors. It doesn’t mean talent isn’t there.”**  


# The numbers behind success: a statistical dive


<div style="text-align: center; margin-bottom: 20px;">
    <img 
        src="{{ '/assets/plots/correlation.png' | relative_url }}" 
        width="100%" 
        height="600px" 
        alt="Feature Correlation Heatmap"
        style="border: 1px solid #ccc; padding: 10px;" />
</div>


The Sigma Squad's journey to uncover the secrets of success in the film industry culminated in this comprehensive correlation heatmap. It serves as the final data-driven map of relationships between various factors and their influence on actors' success. Here’s what they uncovered:

1. **Height and Birth Year**: a moderate negative correlation between **height** and **birth year** suggests that taller individuals are slightly more prevalent among older generations of actors. Pol joked, "Maybe being tall was the superhero casting requirement back then!"

2. **Age at First Release and Birth Year**: a strong negative correlation between **age at first release** and **birth year** reflects how younger actors tend to start their careers earlier in modern times, aligning with changing industry dynamics. Mathieu remarked, "It’s all about hitting the ground running these days."

3. **Success Score Correlation**: surprisingly, the **success score** shows weak correlations with most features. This highlights that success is not dominated by a single attribute but is likely influenced by a blend of multiple factors and intangible qualities like talent and luck. Elise noted, "So success really is the sum of all parts—and a little bit of magic."

4. **University Rankings**: a strong inverse relationship between **ranked universities** and **usable university rank** confirms that higher-ranked universities offer a slight edge in success. However, the weak correlation with success itself suggests that education helps but doesn’t guarantee stardom. Maël quipped, "Turns out, charisma beats calculus in Hollywood."

5. **Specialized Schools**: among specialized schools, **drama schools** stand out with a slight positive correlation to success. Other schools, such as **acting** or **arts schools**, show no significant impact, emphasizing the value of focused dramatic training. Aiden added, "It looks like drama schools teach more than drama—they teach determination."

6. **Number of Children**: a weak positive correlation between **number of children** and **success score** could hint at personal stability or life choices playing a role. Mathieu playfully speculated, "So having kids makes you grounded—literally and figuratively."




As the team analyzed the data, it became clear that success in the film industry is a multifaceted and highly diverse phenomenon. While some trends emerge, like the benefits of drama schools or the importance of starting young, no single factor dominates. Success remains a mix of preparation, opportunity, and the ever-elusive element of luck.


This heatmap and its analysis mark the final chapter of the Sigma Squad’s data journey. Aiden summarized it best, **"Our heatmap shows the threads of the story but not the entire tapestry. And that's what makes this journey so exciting—there's always more to discover!"**

### Next : [A conclusion from all these insights! ]({{ '/conclusion/' | relative_url }})
