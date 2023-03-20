<template>
  <div class="tweet-container">
    <Employees v-for="tweet in tweets" :tweet="tweet" :key="tweet.id"/>
  </div>
</template>

<script>
import Employees from './Employees.vue';
const tweets = [
  {
    id: 1,
    name: 'James',
    handle: '@jokerjames',
    img: 'https://semantic-ui.com/images/avatar2/large/matthew.png',
    tweet: "If you don't succeed, dust yourself off and try again.",
    likes: 10,
  },
  { 
    id: 2,
    name: 'Alina',
    handle: '@fantasticAlina',
    img: 'https://semantic-ui.com/images/avatar2/large/molly.png',
    tweet: 'Better late than never but never late is better.',
    likes: 12,
  },
  { 
    id: 2,
    name: 'Aimen',
    handle: '@AimanTweets',
    img: 'https://cdn.pixabay.com/photo/2017/04/30/11/42/hijab-2272708__340.png',
    tweet: 'My life my rules',
    likes: 42,
  },
  { 
    id: 2,
    name: 'Sandy',
    handle: '@sandyDays',
    img: 'https://cdn.pixabay.com/photo/2020/11/22/22/17/male-5768177__340.png',
    tweet: 'Just play it hard until it really gets you going..........',
    likes: 13,
  },
  {
    id: 3,
    name: 'Xin',
    handle: '@xeroxin',
    img: 'https://semantic-ui.com/images/avatar2/large/elyse.png',
    tweet: 'Beauty in the struggle, ugliness in the success.',
    likes: 18,
  },
  {
    id: 4,
    name: 'John',
    handle: '@johhn',
    img: 'https://cdn.pixabay.com/photo/2016/08/20/05/38/avatar-1606916__340.png',
    tweet: 'Hard work pays off',
    likes: 180,
  }
]

export default {
  components: {
    Employees
  },
  data: function () {
    return { tweets }
  },
}
</script>

<style>
.tweet-container {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    padding: 2rem;
}
</style>