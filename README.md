![Logo Swapcard](./assets/logo_swapcard.svg)

# React technical test

## Introduction

Goal is to build a small app to search musical artists from this GraphQL API endpoint <https://graphbrainz.herokuapp.com>.
No authentication is required.
You should be able to locally set/unset artists as "favorites".
The project must be versioned, hosted and publicly available on a git forge.
It would be great that the project run online ([herokuapp](https://www.heroku.com) / [netlify](https://www.netlify.com)) but it's not mandatory.

_Using GraphQL is a must have, but if you can't, feel free to use another similar REST API_

## The product you must build

- **Home page** :
  List artists depending of a search
  (
  watchout empty search will throw an error from the api,
  so make a UI that display an empty view when no search
  and the results list if search is filled
  )
- **Artist details page** :
  display in a "nice" UI primary informations of the selected artist and a small list of some of the artist's releases.
  From this view, the user must be able to set/unset an artist as favorites.
- **Layout** (displayed on both pages) :
  - Add a way to go back from a details to the list (breadcrumb, menu, buttons, etc...).
  - Sidebar : That will contain your "favorites" artists.

## Nice to have

This part is not mandatory,
it's only some suggestions to improve your test,
you can of course add other part yourself instead of the list below.

- Debounce your search to prevent api flood.
- Add a toast `{{artist}} has been added to your favorites`.
- Create another subpage for Artist's albums (Artist -> Album -> Details).
- Give a try to an SSR (Server Side Rendering) first initial render.
- Infinite scrolling in the artists list.

## Some tools you could use

- React (mandatory)
- For handling data fetching,
  you can work with `react-apollo`, `react-delay`
  or your own implementation of fetch using graphql.
- For handling local data (user "favorite" artists),
  you can work with redux, react context, localStorage, apollo local schema, etc...
- You can type your code using typescript or flow
- You can bootstrap your app using react-create-app
- For styling, use any framework / library you want
  (styled-component, grommet, material, ...)
- if you're aware of this, you can use React Hooks
