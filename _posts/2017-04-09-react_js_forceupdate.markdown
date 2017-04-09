---
layout: post
title:  "React.js: forceUpdate()"
date:   2017-04-09 22:29:07 +0000
---


I remember my first day of learning React.js: learning about Components, their properties and state. I had a task to create a button where onClick will update state. Without any knowledge, I naively typed this.state.key = updatedKey and expected that to work. I found that nothing was changed and it was then I had to ask my AMAA (Ask Me Anytime) coding mentor: Google how to update this.state (and yes I was too dumb to read the documentation). Surprisingly, the first link I found taught me to add a forceUpdate() post this.state.key = updatedKey.  

I learned shortly after solving the problem that the "proper" solutions to same problem was setState. Reading the react documentation, I found a rather interesting part. It was the setState and the forceUpdate section. Basically, setState() will essentially re-render given that shouldComponentUpdate returns true. The other method, forceUpdate will also cause the component to re-render, but like a boss. The "boss" does not need the opinion of shouldComponentUpdate, he/she will go and re-render as he/she pleases. 

I did some research and found that a vast majority of developers believed that forceUpdate was a hack (lazy man method with potential disasters) and should never be used. A thought came to me everytime, I saw that forceUpdate should not be used. I mean, if there was never a case for forceUpdate to be used, why was it developed in the first place. Refering back to the React documentation, there was 1 quote: "Normally you should try to avoid all uses of forceUpdate() and only read from this.props and this.state in render()". 

Facebook's React documentation hinted that was a reason to use forceUpdate. I searched high and low without a good example when to use forceUpdate. I was thinking of forceUpdate as a method that Facebook provided and not a "hack" that was created. The main audiences that this hack appeal to are developers that chose to not maintain a local state. Then there are certain developers with a deadline coming up and they have essential logic in shouldComponentUpdate stopping them from using setState.
