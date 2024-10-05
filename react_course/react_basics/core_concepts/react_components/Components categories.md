![[Components categories.png]]

###### In components separation there are 3 types of ways to split the UI components they are
- Stateless /Presentational component 
- Stateful components
- Structural components

##### Stateless /Presentational component 
```
function Logo() {

return (
<div className="logo">
<span role="img">🍿</span>
<h1>usePopcorn</h1>
</div>

)}
```
This example code snippet for Stateless /Presentational component which is look like no state for example logo remains same state.

##### Stateful components
```
function Search() {

const [query, setQuery] = useState("")

return (
<input
className="search"
type="text"
placeholder="Search movies..."
value={query}
onChange={(e) => setQuery(e.target.value)}
/>

)}
```
This example code snippet for Stateful components which is look like change state for example search bar.

##### Structural components

```
function Main({movies}) 

return (
<main className="main">
<ListBox movies={movies} />
<WatchedBox />
</main>

)}
```
 This example code snippet for structural component which is look like page and layouts


