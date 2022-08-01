# Mews Technology Radar
Explore the current Mews Technology Radar at <insert url>

## Updating the radar
We use a slightly modified version of the [ThoughtWorks build-your-own-radar](https://github.com/thoughtworks/build-your-own-radar#using-json-data) format.

```typescript
type Blip = {
    /**
     * Blip name used in headings.
     */
    name: string;

    /**
     * See "What are the rings?" in https://www.thoughtworks.com/radar/faq-and-more.
     */
    ring: 'Hold' | 'Trial' | 'Assess' | 'Adopt';

    /**
     * Unlike the rings, the quadrants are mostly just to organize the blips and it's not that important where will individual blips end up.
     * 
     * Coding - Lower level coding practices and guidelines.
     * Architecture - High level code organization and structure approaches.
     * Platforms - What we build our software on. Cloud providers, workflow automation, runtimes...
     * Techniques - Elements of software development process.
     */
    quadrant: 'Coding' | 'Architecture' | 'Platforms' | 'Techniques';

    /**
     * Is this a recent addition to the radar?
     */
    isNew: 'TRUE' | 'FALSE';

    /**
     * GitHub user name of the technical leader championing the blip.
     */
    owner: string;

    /**
     * A paragraph of two of guidance about the blip - the what and why, and where to find more information.
     */
    description: string;
};
```
