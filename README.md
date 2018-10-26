# Just Simple SSG
Attempt to make a very simple static site generator, that allows the addition or substitution of functionality, structure or purpose.

## Core Mission:
- Structure
  - This will only provide an object model to use to build something based on *files*
  - That object model will be used by core and non-core modules and templates
    to create the thing that *you need* without assuming everything about how
    you will use it.
- Focus
  - Data structure and information
  - Separation of parts
- Clarity and 
  - Useful error feedback
  - Clear idea of where things are coming from
- Understandability 
  - Intuitive code and file structure
  - Simple content editing
- Flexibility 
  - Ability to be redefined mostly by user
  - No expectations about usage patterns code or content
- Speed 
  - Design
  - Setup
  - Rendering
- Scalable
  - plan for everything
  - solid data core with simple API

## Not a Priority:

This is an app for local development not a server/application solution. 

- Security
  - This is not a server and will not be connected to external source 
    unless the user has explicit modified it to do so.
- Applications
  - The output of this application is not an application. It produces static
    content. To be used/used an distributed by external things.
- Serving
  - This won't serve. Other applications can be used for that. The plugin/module
    model will allow for timing of other applications to use the content/data it creates
- Influence
  - This app will not intend to push your workflow in any direction. The solution
    will be up to the user. This will only provide an object model to build things
    from files.

## Concept
- Keep the working space clean of files for different users of site
  - App (For Developers)
  - Content (For Developers, and editors)
  - Published (Finished deliverable location)

## Todo
- Try and thingk about how to abstract away from SSG so that it could be used for anything
  - Quick templating
  - Website
  - Website from api
- Focus on structure of content in backend
  - We want to have easy ways to find things in templates
  - We also want easy ways to make things (menus)
  - We want content to be easy to understand
- We want a way to enable canned mode and undefined modes of working with this application
  - We want to be able to quickly make a website
  - We want to build something strange that might not even be a website
- Use modules

## Stages of the application cycle
1. Pre: Time before the application
2. Parse: Create data tree 
2. Modify: Make any changes to the tree before templating
3. Render: Run template methods for output
4. Post: Time after the app is done but hasn't printed the results
5. Complete: Time after the application has finished content is generated

Note: Everything may need to be delayed for unknown async operations. So that
      The user can do what they like, such as analysis and generating items 
      themselves. Or fetching items from other sources.

Speed: Speed will be a second level priority 