<template>
    <div>
        <h1>Agregar</h1>
        <form @submit.prevent="guardarTodo()">
            <div class="mb-3">
                 <label for="nombre" class="form-label">Nombre</label>
                 <input
                    v-model.trim="todo.nombre"
                    type="text"
                    class="form-control"
                    id="nombre"
                    placeholder="Ingrese un nombre"
                    />
            </div>
<hr>
            <div class="form-check form-check-inline">
                <input
                    v-model="todo.Category"
                    class="form-check-input"
                    type="checkbox"
                    id="11"
                    value="Adventure"
                />
                <label class="form-check-label" for="Adventure">Adventure</label>
            </div>

            <div class="form-check form-check-inline">
                <input
                    v-model="todo.Category"
                    class="form-check-input"
                    type="checkbox"
                    id="12"
                    value="Puzzle"
                />
                <label class="form-check-label" for="Puzzle">Puzzle</label>
            </div>

            <div class="form-check form-check-inline">
                <input
                    v-model="todo.Category"
                    class="form-check-input"
                    type="checkbox"
                    id="13"
                    value="Strategy"
                />
                <label class="form-check-label" for="Strategy">Strategy</label>
            </div>

            <div class="form-check form-check-inline">
                <input
                    v-model="todo.Category"
                    class="form-check-input"
                    type="checkbox"
                    id="14"
                    value="Fantasy"
                />
                <label class="form-check-label" for="Fantasy">Fantasy</label>
            </div>

            <div class="form-check form-check-inline">
                <input
                    v-model="todo.Category"
                    class="form-check-input"
                    type="checkbox"
                    id="15"
                    value="Civilization"
                />
                <label class="form-check-label" for="Civilization">Civilization</label>
            </div>

<hr>
            <div class="form-check form-check-inline">
  <input v-model="todo.description" class="form-check-input" type="radio" name="inlineRadioOptions" id="inlineRadio1" value="baja">
  <label class="form-check-label" for="baja">baja</label>
</div>


            <br>
            <button class="btn  btn-success" type="submit">Guardar </button>
        </form>
    </div>
</template>

<script>
export default {
    name: 'Agregar',
    data:()=> {
        return {
            todo:{
                id: '',
                Name: '',
                Publisher: '',
                Category: [],
                Description: '',
                Year: ''
            }
        }
    },
    methods:{
         guardarTodo() {
             console.log("todo", this.todo);
         }
    }
};
</script>