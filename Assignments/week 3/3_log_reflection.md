# Week 3 Log & Reflection

## Audit Table
| Claim | Colour | Check Method | Decision |
| :--- | :--- | :--- | :--- |
| Sweetener D mean is 576.81, median is 167.75, and first-to-last change is 23.83% (149.0 to 184.5)[cite: 5]. | Green | Checked directly against `2_work.ipynb` output[cite: 3, 5]. | Accepted |
| High values may be pulling Sweetener D's mean above its median[cite: 3, 5]. | Amber | Compared mean (576.81) vs median (167.75)[cite: 5]. | Accepted (as a possibility) |
| Suppliers price-gouged buyers during a festival rush. | Red | No festival or supplier-intent data exists in the file[cite: 3]. | Rejected |
| Dropping Staple A's max lowers mean from 158.33 to 110.87 while median stays 112.5[cite: 4, 5]. | Green | Checked second cell output in `2_work.ipynb`[cite: 3, 4]. | Accepted |

## Confused Classmate Excerpt
**Classmate:** Why use 167.75 for Sweetener D when the mean is 576.81? Isn't the mean always the typical price[cite: 5]?  
**Me:** Not when big spikes pull the sum up. For Sweetener D, 576.81 gets dragged up, while 167.75 shows the middle price[cite: 5].  
**Classmate:** But why isn't the average what matters most?  
**Me:** Because a single huge price can warp the mean. In Staple A, removing the top value dropped the mean from 158.33 to 110.87, while the median stayed 112.5[cite: 4, 5].  
**Classmate:** So when is the mean fine to use?  
**Me:** When prices are close together without big spikes, like Pulse C (mean 205.91 vs median 206.00)[cite: 5].

## Reflection
In `1_attempt.md`, I jumped into causes like market shortages and buyer impact that the data doesn't actually prove[cite: 3]. The numbers only show price levels, medians, and first-to-last changes[cite: 3, 5], so I need to keep explanations strictly tentative and stick to what the figures show.