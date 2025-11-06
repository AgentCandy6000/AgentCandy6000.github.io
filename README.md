# Bonsoir

const options = {
  method: 'POST',
  headers: {
    accept: 'application/json',
    'content-type': 'application/json',
    Authorization: 'Bearer eyJhbGciOiJIUzI1NiJ9.eyJhdWQiOiI2MWQ0NGJiOGJhZTQxZDAwMmIyMjUwMjkxNzVlMDBiMSIsIm5iZiI6MTc2MjQ0NzE2OC41ODIsInN1YiI6IjY5MGNjZjQwNzU1ZjVlYzAwYzA3MTcxMiIsInNjb3BlcyI6WyJhcGlfcmVhZCJdLCJ2ZXJzaW9uIjoxfQ.QtgDg6G6UEBjP6MgAZxwECjW0n-HAo_NtRGeb5qdUg0'
  }
};

fetch('https://api.themoviedb.org/3/account/22447080/watchlist', options)
  .then(res => res.json())
  .then(res => console.log(res))
  .catch(err => console.error(err));
