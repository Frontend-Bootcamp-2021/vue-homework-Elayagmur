<template>
  <div class="about">
    <h2 class="page-header">About</h2>
    <p class="about__content">
      <img
        src="https://images.unsplash.com/photo-1552053831-71594a27632d?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=312&q=80"
        alt="About Us"
      />
     The benefits of pets
Most pet owners are clear about the immediate joys that come with sharing their lives with companion animals. However, many of us remain unaware of the physical and mental health benefits that can also accompany the pleasure of snuggling up to a furry friend. It’s only recently that studies have begun to scientifically explore the benefits of the human-animal bond.

Pets have evolved to become acutely attuned to humans and our behavior and emotions. Dogs, for example, are able to understand many of the words we use, but they’re even better at interpreting our tone of voice, body language, and gestures. And like any good human friend, a loyal dog will look into your eyes to gauge your emotional state and try to understand what you’re thinking and feeling (and to work out when the next walk or treat might be coming, of course).

Pets, especially dogs and cats, can reduce stress, anxiety, and depression, ease loneliness, encourage exercise and playfulness, and even improve your cardiovascular health. Caring for an animal can help children grow up more secure and active. Pets also provide valuable companionship for older adults. Perhaps most importantly, though, a pet can add real joy and unconditional love to your life.

Any pet can improve your health
While it’s true that people with pets often experience greater health benefits than those without, a pet doesn’t necessarily have to be a dog or a cat. A rabbit could be ideal if you’re allergic to other animals or have limited space but still want a furry friend to snuggle with. Birds can encourage social interaction and help keep your mind sharp if you’re an older adult. Snakes, lizards, and other reptiles can make for exotic companions. Even watching fish in an aquarium can help reduce muscle tension and lower your pulse rate.

Studies have shown that:

Pet owners are less likely to suffer from depression than those without pets.
People with pets have lower blood pressure in stressful situations than those without pets. One study even found that when people with borderline hypertension adopted dogs from a shelter, their blood pressure declined significantly within five months.
Playing with a dog, cat, or other pet can elevate levels of serotonin and dopamine, which calm and relax.
Pet owners have lower triglyceride and cholesterol levels (indicators of heart disease) than those without pets.
Heart attack patients with pets survive longer than those without.
Pet owners over age 65 make 30 percent fewer visits to their doctors than those without pets.
One of the reasons for these therapeutic effects is that pets fulfill the basic human need for touch. Even hardened criminals in prison show long-term changes in their behavior after interacting with pets, many of them experiencing mutual affection for the first time. Stroking, hugging, or otherwise touching a loving animal can rapidly calm and soothe you when you’re stressed or anxious. The companionship of a pet can also ease loneliness, and most dogs are a great stimulus for healthy exercise, which can substantially boost your mood and ease depression.
    </p>
  </div>
</template>

<script>
import { onMounted, onUnmounted } from "vue";

export default {
  setup() {
    onMounted(() => console.log("Mount: 👓 About Component"));
    onUnmounted(() => console.log("unMount: 👋🏻 About Component "));

    return {};
  },
};
</script>

<style lang="scss">
.about {
  &__content {
    margin: 20px 0;
    padding: 0;

    font-size: 18px;
    line-height: 32px;

    img {
      float: left;

      margin: 0 20px 20px;
    }
  }
}
</style>
