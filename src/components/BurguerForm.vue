<template>
  <div>
    <div>
      <form id="burger-form">
        <div class="input-conteiner">
          <label for="nome">Nome do cliente:</label>
          <input
            type="text"
            id="nome"
            name="nome"
            v-model="nome"
            placeholder="Digite o seu nome"
          />
        </div>

        <div class="input-conteiner">
          <label for="pao">Escolha o pão</label>
          <select name="pao" id="pao" v-model="pao">
            <option value="">Selecione o seu pão</option>
            <option value="integral">Integral</option>
            <option value="wheymorango">Whey de Morango</option>
          </select>
        </div>

        <div class="input-conteiner">
          <label for="carne">Escolha a carne</label>
          <select name="carne" id="carne" v-model="carne">
            <option value="">Selecione o recheio</option>
            <option value="morcego">Asa de morcego</option>
            <option value="pedegalinha">Pé de galinha</option>
          </select>
        </div>

        <div id="opcionais-conteiner" class="input-conteiner">
          <label id="opcionais-title" for="opcionais"
            >Selecione os opcionais:
          </label>
          <div class="checkbox-conteiner">
            <input
              type="checkbox"
              name="opcionais"
              v-model="opcionais"
              value="salame"
            />
            <span>Salame</span>
          </div>
        </div>
        <div class="input-conteiner">
          <input
            type="submit"
            class="submit-btn"
            value="Criar meu Hamburguer"
          />
        </div>
      </form>
    </div>
  </div>
</template>

<script>
export default {
  name: "BurguerForm",
};
</script>

<style scoped>
#burger-form {
  max-width: 400px;
  margin: 0 auto;
}

.input-conteiner {
  display: flex;
  flex-direction: column;
  margin-bottom: 20px;
}

label {
  font-weight: bold;
  margin-bottom: 15px;
  color: #222;
  padding: 5px 10px;
  border-left: 4px solid #fcba03;
}

input,
select {
  padding: 5px 10px;
  width: 300px;
}

#opcionais-container {
  flex-direction: row;
  flex-wrap: wrap;
}

#opcionais-title {
  width: 100%;
}

.checkbox-conteiner {
  display: flex;
  align-items: flex-start;
  width: 50%;
  margin-bottom: 20px;
}

.checkbox-conteiner span,
.checkbox-conteiner input {
  width: auto;
}

.checkbox-conteiner span {
  margin-left: 6px;
  font-weight: bold;
}

.submit-btn {
  background-color: #222;
  color: #fcba03;
  font-weight: bold;
  border: 2px solid #222;
  padding: 10px;
  font-size: 16px;
  margin: 0 auto;
  cursor: pointer;
  transition: 0.5s;
}

.submit-btn:hover {
  background-color: transparent;
  color: #222;
}
</style>
