<template>
  <NeonClock :date="new Date()"/>
  <LunarCalendar :date="new Date()" :refresh="60000" />
  <DisplayInfo @date-click="handleDateClick" >
    <GregCalendar :date="new Date()" />
    <MoonCalendar :date="new Date()" />
  </DisplayInfo>
</template>

<script setup>
import NeonClock from '@/components/NeonClock.vue'
import LunarCalendar from '@/components/LunarCalendar.vue'
import DisplayInfo from '@/components/DisplayInfo.vue'
import GregCalendar from '@/components/GregCalendar.vue'
import MoonCalendar from '@/components/MoonCalendar.vue'
</script>