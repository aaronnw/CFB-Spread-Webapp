<template>
  <div>
    <h1>{{ home_team.name }} vs. {{away_team.name}}</h1>
  </div>
</template>

<script>
export default {
  name: 'GameDisplay',
  props: {
    game_id: String
  },
  data() {
    return {
      time: '',
      location: '',
      tv: '', 
      home_team: {
        name: '',
        record: '',
        primary_color: '',
        secondary_color: '',
        logo: '',

      },
      away_team: {
        name: '',
        record: '',
        primary_color: '',
        secondary_color: '',
        logo: '',
      },
    };
  },
  created() {
    console.log('todo: query team info')
  }
}
</script>