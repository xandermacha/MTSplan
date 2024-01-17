<script lang="ts">
    // let employee_name = '';
    import AddEmployee from "../lib/AddEmployee.svelte";
</script>


<!-- <input bind:value={employee_name} placeholder="enter employee name"/> -->
<main class="container">

    <h1>Create New Schedule</h1>
    
    <!-- <p>employee {employee_name || 'employee'}</p> -->
    
    <div class="row">
        <AddEmployee />
    </div>
</main>