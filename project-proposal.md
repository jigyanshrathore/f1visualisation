# F1 Standings Explorer

## Overview

I would like to make an F1 Standings Explorer web page. Most standings results for F1 are simple points totals that don’t really convey how a season played out. I would like to make a line graph for a given year to show how each driver accumulated points. If you don't know how F1 points are accumulated, I have a short summary below.

I want to make the webpage interactive by letting users click and explore results further. Users will be able to click into a driver and get more detailed results for that year. The driver detail view will show qualifying and finish race position for each race. I would also like to have a race detail view to show driver position changes lap by lap. These interactive graphs are a great example of using JavaScript and an API to create interactive data visualizations.

### How the F1 Championship Works
There are 10 teams and 20 drivers, two drivers per team, that participate in about 20 races per season. Each race, the top 10 positions are awarded points, with the 25 points going to the winner and the 10th place driver getting a single point. The driver with the most points at the end of the season wins the World Driver's Championship. The team with the most points, combining both drivers, wins the World Constructors's Championship.

Over the course of a weekend drivers participate in Friday practice, Saturday Qualifying, and Sunday race. Qualifying doesn't give points but it determines where you start on race day. Fans place a lot of emphasis on how well drivers qualify but the race finish is where points are awarded. Both are important and tell their own story.

### Race Finish Points Breakdown
| Position | Points |
| - | - |
| 1st | 25 |
| 2nd | 18 |
| 3rd | 15 |
| 4th | 12 |
| 5th | 10 |
| 6th | 8 |
| 7th | 6 |
| 8th | 4 |
| 9th | 2 |
| 10th | 1 |

## Functionality and Features
F1 Standings Explorer will provide interactive data visualizations for users to explore and get a high level overview of how a F1 season played out.

### Main Page: Season Summary
The main page will be a line graph to summarize points earned over the course of the season per driver. It will have the option select different years, filter drivers, filter teams, give a start date and end date to adjust the x-axis, and toggle between the Driver's Championship and the Constructor's Championship.

The x-axis represents the results from a given race. The y-axis represents the points total and each driver will be a different color respective to team colors. For example, Ferrari's Charles Leclerc will be red like his team and the second driver will be a lighter shade of red. Each team has generally distinct colors. If the graph is crowded users can filter out drivers or teams.

### Driver Detail View: Season Summary with Qualifying Results and Race Finish
Users will be able to click on a driver from the main page to pull up a more in depth view for just that driver. This graph will show qualifying results along with race finish for each race. This view is useful for seeing if a driver typically finishes where they qualify. Some drivers drop down the order while others climb up the field.

The x-axis still represents each race but I'll have two bar charts per race to show where they qualified and where they finished. The y-axis still represents the points total over the course of the season. I'll add a line graph on top of the bar chart.

