<script lang='ts'>
    import { invoke } from "@tauri-apps/api/tauri"

    let employeeName = "";
    let employeeAddMsg = ""

    async function addEmployee(){
        // Learn more about Tauri commands at https://tauri.app/v1/guides/features/command
        employeeAddMsg= await invoke("add_employee", { employeeName })
    }
</script>
<div>
    <form class="row" on:submit|preventDefault={addEmployee}>
      <input id="employee-input" placeholder="Enter employee name" bind:value={employeeName} />
      <button type="submit">Add</button>
    </form>
    <p>{employeeAddMsg}</p>
  </div>