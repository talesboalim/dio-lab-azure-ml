# Trabalhando com Machine Learning na Prática no Azure ML
https://web.dio.me/lab/trabalhando-com-machine-learning-na-pratica-no-azure-ml
1. Criar uma conta na azure.microsoft.com
1. Criar um recurso no Azure Machine Learning
1. Acessar ml.azure.com
1. Acessar Create workspace
1. Criar um novo workspace
1. Selecione o workspace criado
1. No menu selecione ML Automatizado
1. Selecione New Atomated ML job
1. Informe no Job name: dio-lab-ml-ibpt
1. New experiment name: dio-lab-ml-ibpt
1. Selecione Next
1. Em Select task type selecione Regression
1. Selecione Create
1. Em name informe ibpt
1. Em Type selecione Tabular
1. Selecione Next
1. Selecione From local files
1. Pressione Next
1. Em Datastore type selecione Azure Blob Storage
1. Pressione Next
1. Pressione Upload files or folder
1. Baixe a última versão da tabela de IBPT de SP em CSV(https://deolhonoimposto.ibpt.org.br/)
1. Selecione o arquivo TabelaIBPTaxSP24.1.A.csv
1. Pressione Next
1. Na aba Settings será identificado o conteúdo do arquivo, não precisa modificar nenhuma opção
1. Pressione Next
1. Em Schema, pressione Next
1. Em Review, pressione Create
1. Aguarde a tarefa ser executada. 
1. Em Task Type & data, selecione ibpt
1. Pressione Next
1. Em task Settings, Target column selecione nacionalfederal.  Desmarque Explain best model e Use all supported models em View additional configuration settings. e também selecione os modelos RandomForest e LightGBM. Pressione Save.
1. Em limits, informe 3 para Max trials, concurrent trials, nodes. Em metrics 0,085. Em Experiment timeout e Iteration informe 15. Marque Enable early termination.
1. Em validation type, selecione Train-validation split.
1. Pressione Next
1. Em compute, pressione Next.
1. Em review, pressione Submit training job.
1. Aguarde a conclusão da tarefa. Você pode acompanhar o processo no menu Jobs.
1. O status do Job deve estar Completed.
