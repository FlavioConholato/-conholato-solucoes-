<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <title>Conversor BOPM para Padrão CPRv</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #f4f4f4;
      padding: 20px;
    }
    textarea {
      width: 100%;
      height: 300px;
      font-family: monospace;
      margin-bottom: 15px;
    }
    button {
      padding: 10px 20px;
      background-color: #1e88e5;
      color: white;
      border: none;
      cursor: pointer;
      margin-right: 10px;
    }
    .output {
      white-space: pre-wrap;
      background: #fff;
      padding: 15px;
      border: 1px solid #ccc;
      margin-top: 20px;
    }
  </style>
</head>
<body>

<h2>Conversor BOPM para Padrão CPRv</h2>

<textarea id="entrada" placeholder="Cole aqui o texto bruto (X)..."></textarea>
<br>
<button onclick="converter()">Converter</button>
<button onclick="baixarTXT()">Baixar como .txt</button>

<div class="output">
  <strong>Padrão CPRv Gerado:</strong><br><br>
  <textarea id="saida" readonly style="height: 400px;"></textarea>
</div>

<script>
function converter() {
  let texto = document.getElementById("entrada").value;

  // 🔥 Remover blocos desnecessários
  texto = texto.replace(/LANÇADO PELO APLICATIVO[\s\S]*?registro:[^\n]*\n?/i, '');
  texto = texto.replace(/Comunicação de Ocorrência Policial[\s\S]*?registro:[^\n]*\n?/i, '');
  texto = texto.replace(/Apreensões[\s\S]*?Veículos Envolvidos/i, '');
  texto = texto.replace(/Endereço[\s\S]*?Guarnição\/Policiamento/i, '');
  texto = texto.replace(/Envolvidos[\s\S]*?Brat/i, '');
  texto = texto.replace(/Brat[\s\S]*?Condutor:/i, '');

  // Dinâmica
  let historico = "---";
  const dinamicaMatch = texto.match(/Declaração:\s*(.*)/i);
  if (dinamicaMatch) {
    historico = dinamicaMatch[1].trim();
  }

  // Observações
  let observacoes = "---";
  const obsMatch = texto.match(/Condutor:[^\n]*\n([\s\S]*)/i);
  if (obsMatch) {
    observacoes = obsMatch[1].trim();
  }

  const textoY = `SECRETARIA DE ESTADO DE POLÍCIA MILITAR

COMANDO DE POLICIAMENTO RODOVIÁRIO (CPRv)

5ª CTRv - POSTO PPRv


TERMINO DE OCORRÊNCIA

DATA: 

HORA INICIAL: 
HORA FINAL:  

LOCAL: 


LINK GEORREFERENCIADO:


CÓD. INICIAL: 

CÓD. FINAL: 

BOPM: CPRV
RO: 
DP:  
BRAT:
Protocolo: 

QUALIFICADOS:

A1:
CPF: 
CNH:
CAT:
VAL: 
DN: 
BAM: 


VEÍCULO ENVOLVIDO: 

(V1) 
MARCA/MODELO: 
PLACA: 
COR: 
ANO: 

EQUIPE: 

VTR: 

DINÂMICA / HISTÓRICO:
${historico}

OBSERVAÇÕES:
${observacoes}
`;

  document.getElementById("saida").value = textoY;
}

function baixarTXT() {
  const texto = document.getElementById("saida").value;
  const blob = new Blob([texto], { type: "text/plain" });
  const link = document.createElement("a");
  const hoje = new Date().toISOString().split("T")[0];
  link.download = `termino_ocorrencia_${hoje}.txt`;
  link.href = URL.createObjectURL(blob);
  link.click();
}
</script>

</body>
</html>
