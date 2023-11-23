<template>
  <div>
    <div class="project-title-container">
      <div class="content-wrapper">
        <div class="title-text">
          <span>Power BI Project</span>
        </div>

        <div class="description-text">
          <p>
            O seguinte dashboard foi minuciosamente projetado para proporcionar uma visão abrangente e detalhada sobre restaurante localizados na região Sudeste do Brasil, destacando aspectos cruciais relacionados a eles. Ao navegar por este painel interativo, os usuários terão acesso a um conjunto de informações sobre diversas categorias de restaurantes, suas localidades, avaliações e médias de custo.
          </p>
          <p>
            A primeira seção do dashboard concentra-se nos seus dados de identificação,  como nome, endereço, estado e cidade, permitindo uma análise aprofundada por região. Os usuários poderão explorar diferentes especialidades, desde culinárias internacionais até opções de fast food, proporcionando uma compreensão abrangente do cenário gastronômico representado.
          </p>
          <p>
            A geolocalização dos restaurantes é crucial para entender a distribuição e a acessibilidade. O dashboard oferece recursos interativos para mapear a presença dos restaurantes em diferentes regiões, facilitando uma análise visual e identificação de padrões.
          </p>
          <p>
            A seção de avaliações destaca a qualidade percebida pelos clientes, proporcionando uma visão instantânea das experiências passadas. Gráficos intuitivos e métricas consolidadas permitem identificar padrões de satisfação do cliente e áreas de melhoria.
          </p>
          <p>
            A análise das médias de custo oferece uma perspectiva para proprietários de restaurantes e clientes, fornecendo insights sobre os diferentes segmentos de preço.
          </p>
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
    gap: 12px;
    font-weight: 300;
    margin-bottom: 20px;
    max-width: 900px;
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