# TaNaMesa-data-pipeline

<p>Utilizamos este repositório para definir o pipeline de dados utilizado para monitoramento em tempo real da política pública TáNaMesa<br>
O monitoramento da operacionalização desta política pública ocorre através da aplicação de um questionário digital respondido pelos beneficiários do programa.</p>

### Descrição do pipeline geral

<p>Para definir as perguntar que iriam compôr o questionário, realizou-se um cuidados estudo de caso. Os documentos
mais importantes, como edital de credenciamento e lei definidora, foram estudados para que montássemos as perguntas
mais consistentes e relevantes possíveis.</p>
<p>Além disso, usamos o software de questionário digital Tally, para aplicar e gerar o QR-CODE de acesso às perguntas.</p>
<p>As respostas são colhidas via script Python e tratadas antes de formarem a base de dados online, que será consumida pelo Metabase para disposição do dashboard de Business Intelligence.</p>
<p>A base de dados online gratuita escolhida foi o Retool, com 5 GB de armazenamento disponível gratuitamente.</p>
<p>O metabse checa a engine PostgreSQL hospedado pelo Retool e monta os KPI que definimos junto com as perguntas do questionário.</p>
