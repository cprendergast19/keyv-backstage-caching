# How to Implement Caching in Backstage

## What is Backstage?
Backstage is an open platform for building developer portals to centralize tooling, software components, data, and documentation for developers.

## Example - Add Cache Support to Backstage.io

Install whichever storage adapter you will be using, keyv-redis in this example
`npm install --save keyv-redis`

Create an Instance of Keyv with caching support
```js
backend:
  cache:
  	store: keyv-redis
		connection: new Keyv('redis://user:pass@localhost:6379')
```
