<script setup>
const firstPerson = {
  gender: 'female',
  firstname: 'Emily',
  lastname: 'Parker',
  age: 24,
  job: 'Teacher',
  hobbies: ['read books', 'go hiking'],
  pet: {
    name: 'Whiskers',
    age: 2,
    species: 'ferret'
  }
}

const secondPerson = {
  gender: 'male',
  firstname: 'Marcus',
  lastname: 'Bennett',
  age: 38,
  job: 'Architect',
  hobbies: ['watch bird', 'play chess'],
  pet: {
    name: 'Nala',
    age: 6,
    species: 'dog'
  }
}

const thirdPerson = {
  gender: 'female',
  firstname: 'Sophia',
  lastname: 'Rodriguez',
  age: 31,
  job: 'Environmental scientist',
  hobbies: ['play guitar', 'bake cakes'],
  pet: {
    name: 'Paws',
    age: 3,
    species: 'cat'
  }
}

const fourthPerson = {
  gender: 'male',
  firstname: 'Oliver',
  lastname: 'Hughes',
  age: 56,
  job: 'Carpenter',
  hobbies: ['paint', 'ride horses'],
  pet: {
    name: 'Bubble',
    age: 4,
    species: 'snake'
  }
}
</script>

<template>
  <main>
    <h1>Description list</h1>
    <div class="cards">
      <div>
        <img src=".//assets/imgs/persons/emily-parker.jpg" alt="" />
        <h2>{{ firstPerson.firstname }} {{ firstPerson.lastname }}</h2>
        <p>She is a {{ firstPerson.age }}-year-old {{ firstPerson.job }}.</p>
        <p>
          Outsise of work, {{ firstPerson.firstname }} likes to {{ firstPerson.hobbies[0] }} and
          {{ firstPerson.hobbies[1] }}.
        </p>
        <p>
          At home, her lively companion is {{ firstPerson.pet.name }} a
          {{ firstPerson.pet.age }}-years-old {{ firstPerson.pet.species }}.
        </p>
      </div>

      <div>
        <img src=".//assets/imgs/persons/marcus-bennett.jpg" alt="" />
        <h2>{{ secondPerson.firstname }} {{ secondPerson.lastname }}</h2>
        <p>He is a {{ secondPerson.age }}-year-old {{ secondPerson.job }}.</p>
        <p>
          Outsise of work, {{ secondPerson.firstname }} likes to {{ secondPerson.hobbies[0] }} and
          {{ secondPerson.hobbies[1] }}.
        </p>
        <p>
          At home, her lively companion is {{ secondPerson.pet.name }} a
          {{ secondPerson.pet.age }}-years-old {{ secondPerson.pet.species }}.
        </p>
      </div>
      <div>
        <img src=".//assets/imgs/persons/sophia-rodriguez.jpg" alt="" />
        <h2>{{ thirdPerson.firstname }} {{ thirdPerson.lastname }}</h2>
        <p>She is a {{ thirdPerson.age }}-year-old {{ thirdPerson.job }}.</p>
        <p>
          Outsise of work, {{ thirdPerson.firstname }} likes to {{ thirdPerson.hobbies[0] }} and
          {{ thirdPerson.hobbies[1] }}.
        </p>
        <p>
          At home, her lively companion is {{ thirdPerson.pet.name }} a
          {{ thirdPerson.pet.age }}-years-old {{ thirdPerson.pet.species }}..
        </p>
      </div>
      <div>
        <img src=".//assets/imgs/persons/olivier-hughes.jpg" alt="" />
        <h2>{{ fourthPerson.firstname }} {{ fourthPerson.lastname }}</h2>
        <p>He is a {{ fourthPerson.age }}-year-old {{ fourthPerson.job }}.</p>
        <p>
          Outsise of work, {{ fourthPerson.firstname }} likes to {{ fourthPerson.hobbies[0] }} and
          {{ fourthPerson.hobbies[1] }}.
        </p>
        <p>
          At home, her lively companion is {{ fourthPerson.pet.name }} a
          {{ fourthPerson.pet.age }}-years-old {{ fourthPerson.pet.species }}.
        </p>
      </div>
    </div>
  </main>
</template>

<style scoped>
main {
  display: flex;
  flex-direction: column;
  align-items: center;
}
.cards {
  display: flex;
}

.cards div {
  /* border: 1px solid red; */
  margin: 10px;
  padding: 10px;
  background-color: white;
  border-radius: 10px;
  box-shadow: 0px 0px 4px 0px rgba(0, 0, 0, 0.25);
  height: 500px;
  width: 300px;
}

img {
  width: 100%;
  max-height: 35%;
  border-radius: 10px;
  margin-bottom: 20px;
  object-fit: cover;
  object-position: center top;
}
</style>
