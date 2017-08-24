# React Rally 2017 Notes
Notes and Examples from React Rally 2017 in Salt Lake City, UT.<br>
http://www.reactrally.com/

## Day 1

### Unpkg - Michael Jackson - 9:00 AM
Speaker: [Michael Jackson](https://github.com/mjackson)<br>
Topic: Unpkg.com<br>
Twitter: [@unpkg](https://twitter.com/unpkg)<br>
Demos: https://github.com/unpkg/unpkg-demos<br>
Local: [unpkg-demos](unpkg-demos) <br>

**Notes:**
- What is it?
    - Global CDN for everything on npm
    - Quickly and easily load any file from any package
- Module support is coming to browsers

*"Just imagine what a cool world it would be if everyone only loaded React once..."*

### D3 and React - Shirley Wu - 9:30 AM
Speaker: [Shirley Wu](https://github.com/sxywu)<br>
Topic: D3 and React<br>
Presentation Link: https://github.com/sxywu/react-d3<br>
Local: [react-d3](react-d3) <br>

**Notes:**
- Data visualization
- Who *needs* control of the DOM?
- D3 only needs the DOM in 3 places
    + transitions (x,y position, color changes, etc.)
    + axes (we tell D3 what we want, it updates for us)
    + brushes (event binding)
- D3 doesn't need the DOM for
    + layouts
    + geo
    + shape
- React renders, D3 calculates
- D3 is more than enough for hover, click, and other simple interactions. React comes in handy for more complicated UIs and interactions.
- Use React with D3 when you need to manage state in your app
- When React renders
    + if user interaction *does* mutate data
    + propagates from parent
    + calculate in `componentWillReceiveProps`

### React for IOT - Devon Lindsey - 10:30 AM
Speaker: [Devon Lindsey](https://github.com/devonbl) <br>
Topic: A Hand Wave of React for All Your Internet of Thangs <br>
Twitter: [@devonbl](https://twitter.com/devonbl) <br>
Presentation Link: N/A <br>
Local: N/A <br>

**Notes:**
- What the heck is NFC? Near Field Communication
    + EX: Card that is used for mass transit, work badge, etc.
- What NFC is **not**
    + A tracking device
- "I have an NFC implant in my hand, I want to wire it up to my house using IOT technology" 😳
- Random fact: Arduino != Raspberry Pi
    + Raspberry Pi entry barrier is much lower - it has an awesome community
    + See: https://github.com/raspberrypi
- Technologies Used:
    + Johnny Five: http://johnny-five.io/ - used for IOT
    + raspi-io: https://github.com/nebrius/raspi-io - Provides IO for Johnny-Five on Raspberry Pi
    + react-hardware: https://github.com/iamdustan/react-hardware

**TLDR**: This woman literally put an NFC chip in her hand so she can unlock her house by swiping her hand... because old school keys are overrated. Pretty intense stuff.

### Back to React - Michael Chan - 11:00 AM
Speaker: [Michael Chan](https://github.com/chantastic) <br>
Topic: Back to React: The Story of Two Apps <br>
Twitter: [@chantastic](http://twitter.com/chantastic) <br>
Presentation Link: N/A <br>
Local: N/A <br>

**Notes:**
- React represents the V in MVC frameworks
- Easy to plug components into an application
- Why React is great
    + Big components + better patterns
    + Context
    + inline-styles + CSS
    + RTFM + nothing else existed

- 5 Important Keys to Being a React Developer:
    + 1. Know who's driving
        * In order to be a React developer, you need to know the following (Holy Trinity of React):
            - React
            - React-router
            - Redux
            - React-router-redux
        * It's getting more and more complicated, which is a possible deterrent for people looking into using React
        * What role does react play in your app?
    + 2. Optimize for change
    + 3. Know your component shapes (master the patterns)
    + 4. Avoid the edges
        * "Dont forget it's not the edge that's bleeding, it's you."
        * If you're the one using bleeding edge technology, you'll be feeling the pain
    + 5. Partner, don't depend
        * "Debugging is twice as hard as writing the code in the first place. Therefore, if you write the code as cleverly as possible, you are, by definition, not smart enough to debug."
        * Stop delegating
