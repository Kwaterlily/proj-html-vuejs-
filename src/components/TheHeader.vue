<template>
  <header>
    <nav>
        <ul>
            <li v-for="link in links" :key="link.id">
                <a :href="link.url" :class="{ active: link.active }">
                    {{ link.text }}  {{ link.day }} {{ link.hour }}
                </a>
            </li>
            <li v-for="link in links" :key="link.id">
                <a :href="link.url" :class="{ active: link.active }">
                    {{ link.phone_icon }}  {{ link.number }} {{ link.mail_icon }}
                    {{ link.mail }} {{ link.f_icon }} {{ link.t_icon }} {{ link.l_icon }}
                </a>
            </li>
        </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name: 'TheHeader',
  props: {
    links: Array
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>


