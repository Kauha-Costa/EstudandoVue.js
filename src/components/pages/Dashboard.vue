<script setup>
    import Grid from '../Grid.vue'
    import { gymHealthFacts } from '../../utils'

    // generate a random integer number between 0 and the length -1 of the gymHealthFacts array
    const randomNumber = Math.floor(Math.random() * gymHealthFacts.length)
    const todaysFact = gymHealthFacts[randomNumber]

</script>

<template>
    <section id="dashboard">
        <div class="card tip-container">
            <h2>Welcome Forger</h2>
            <div>
                <p class="tip"><strong>Daily Tip</strong><br>{{  todaysFact }}</p>
            </div>
            <button>Start Workout &rarr;</button>
        </div>
        <Grid/>
    </section>
</template>

<style scoped>

    .tip-container,
    .tip-container div,
    #dashboard{
        display: flex;
    }

    .tip-container,
    #dashboard{
        flex-direction: column;
    }

    #dashboard{
        gap: 2rem;
    }

    .tip-container{
        gap: 0.5rem;
    }

    @media (min-width: 640px) {
        .tip-container{
            gap: 1rem;
        }
    }
</style>
