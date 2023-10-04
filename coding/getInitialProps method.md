
it is a [[method]] that is available in the next [[framework]], it allows me to fetch data for a component or a the root of a project during the build process in the server.

I should call this method in the file where I am defining the component that I am going to use it on, it follows this pattern: ComponentName.getInitialProps( () => {
const data = get data from API

return data;
})

This example would return data to the ComponentName component as a prop.