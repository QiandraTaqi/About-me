<template>
  <div class="container">
    <div 
      class="envelope-wrapper" 
      :class="{ open: isOpen }" 
      @click="isOpen = !isOpen"
    >
      <div class="envelope">
        <div class="front flap"></div>
        <div class="front pocket"></div>
        <div class="letter" @click.stop>
          <div class="letter-content">
            <h2>Happy "Late" Birthday Hanifa!</h2>
            <p>
              Happy 16th birthday, sorry for the late suprise XD  (you know). Uhhh,,, i honestly dont know what to say. Its almost a year since we first "talked".  But i hope you can pass all ur hard time, i hope you can graduate from SI with a smile. I hope you can go to ur dream college, be rich and a cool aunt. I remember you chat me out of nowhere and yap about ur "FRIENDSHIP" with Ihsan.
            </p>
            <p>
              I want to say thank you for all ur help for these past year, you've been helping me much even without you know it. And im also feel sorry if i ever crossed the line when joking with you, and im sorry if i cant be a good listener and cant help you much, im not good at giving advice, im so sorry
            </p>
            <p>
              You're.. the most toughest woman (beside my mom) that i ever met tbh. You got all those problem carrying on you (altaf, ur relaiton with isan, iwan, SI, etc) but yet, you still able to continue living, you still be able to move forward and continue another day. You've worked hard. i hosently dont know what else to say XD. But yeah, thanks once again for these one year and also for the es oyen, enak.
            </p>
            <p>Peace Out</p>
            <p class="signature">Wish you all the bset<br>Qoqoy</p>
          </div>
        </div>
      </div>
    </div>
    <p class="hint">{{ isOpen ? 'Click outside to close' : 'Click the envelope to open' }}</p>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const isOpen = ref(false)
</script>