<template>
  <div>
    <div class="project-title-container">
      <div class="content-wrapper">
        <div class="title-text">
          <span>Sobre</span>
        </div>

        <div class="description-text">
          <div class="description-info">
            <span class="title">Disciplina:</span>
            <span class="info">Business Intelligence</span>
          </div>

          <div class="description-info">
            <span class="title">Universidade:</span>
            <span class="info">Pontifícia Universidade Católica de Minas Gerais</span>
          </div>

          <div class="description-info">
            <span class="title">Orientador:</span>
            <span class="info">Clóvis Lemos Tavares</span>
          </div>

          <div class="description-info-2">
            <span class="title">Alunos:</span>
            <ul>
              <li class="info">Maria Luisa Couto Fernandes</li>
              <li class="info">Matheus Gabriel G Cunha de Oliveira</li>
            </ul>
          </div>
        </div>
      </div>

      <div class="title-buttons">
        <button @click="$router.push('/project')">
          Ver projeto
        </button>
      </div>
    </div>
  </div>
</template>

<style scoped>
  .project-title-container {
    display: flex;
    align-items: center;
    flex-direction: column;
    margin-top: 16vh;
    gap: 16px;
    height: 60vh;
  }

  .att-info-container {
    display: flex;
    justify-content: flex-end;
    height: 40vh;
  }

  .info-area {
    display: flex;
    flex-direction: column;
    text-align: end;
  }

  .title-text {
    font-size: 74px;
    font-weight: 500;
    display: flex;
    gap: 18px;
  }

  .content-wrapper {
    background: rgba(255, 255, 255, 0.1);
    border-radius: 8px;
    box-shadow: 0 4px 30px rgba(0, 0, 0, 0.1);
    backdrop-filter: blur(4.4px);
    -webkit-backdrop-filter: blur(4.4px);
    border: 1px solid rgba(255, 255, 255, 0.1);

    display: flex;
    flex-direction: column;
    gap: 16px;
    align-items: center;
    padding: 16px;
  }

  .description-text {
    display: flex;
    flex-direction: column;
    gap: 8px;
  }

  .description-info {
    display: flex;
    gap: 12px;
  }

  .description-info-2 {
    display: flex;
    gap: 26px;
  }

  .title {
    font-weight: 600;
  }

  .info {
    font-weight: 300;
  }

  button {
    background: rgba(255, 255, 255, 0.1);
    border-radius: 6px;
    box-shadow: 0 4px 30px rgba(0, 0, 0, 0.1);
    backdrop-filter: blur(4.4px);
    -webkit-backdrop-filter: blur(4.4px);
    border: 1px solid transparent;
    color: white;
    font-size: 18px;
    padding: 10px;
    transition: all .2s;
    cursor: pointer;
  }

  button:hover {
    transform: scale(1.1) rotate(3deg);
  }
</style>