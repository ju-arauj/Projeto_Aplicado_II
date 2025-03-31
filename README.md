# Projeto_Aplicado_II
📊 Análise de Sentimentos em Avaliações de Produtos da Sephora

📌 Sobre o Projeto

A Sephora é uma das maiores redes de cosméticos do mundo. Neste projeto, analisamos avaliações de clientes sobre produtos de skincare, aplicando análise de sentimentos para classificá-las como positivas, negativas ou neutras. O objetivo é entender a recepção dos produtos e identificar fatores que influenciam a satisfação dos consumidores.

📂 Fonte e Dados

Os dados foram obtidos do Kaggle e incluem:

Produtos e marcas

Preços e ingredientes

Mais de 1 milhão de avaliações de skincare

Data da avaliação e características dos usuários

Classificações feitas por outros usuários

Os dados estão organizados em arquivos CSV.

Link do datasets utilizados: https://www.kaggle.com/datasets/nadyinky/sephora-products-and-skincare-reviews/data

📂 Metadados
 ### Conteúdo do product_info

**Recurso** | **Descrição**  
--- | ---  
**product_id** | O identificador único do produto no site.  
**product_name** | O nome completo do produto.  
**brand_id** | O identificador único da marca do produto no site.  
**brand_name** | O nome completo da marca do produto.  
**loves_count** | O número de pessoas que marcaram este produto como favorito.  
**rating** | A classificação média do produto com base nas avaliações dos usuários.  
**reviews** | O número de avaliações dos usuários para o produto.  
**size** | O tamanho do produto, que pode estar em oz, ml, g, pacotes ou outras unidades, dependendo do tipo de produto.  
**variation_type** | O tipo de parâmetro de variação do produto (ex.: Tamanho, Cor).  
**variation_value** | O valor específico do parâmetro de variação do produto (ex.: 100 mL, Golden Sand).  
**variation_desc** | Uma descrição do parâmetro de variação do produto (ex.: tom para pele mais clara).  
**ingredients** | Uma lista de ingredientes incluídos no produto. Exemplo: `['Variação do produto 1:', 'Água, Glicerina', 'Variação do produto 2:', 'Talco, Mica']` ou, se não houver variações, `['Água, Glicerina']`.  
**price_usd** | O preço do produto em dólares americanos.  
**value_price_usd** | A economia potencial do produto, apresentada no site ao lado do preço regular.  
**sale_price_usd** | O preço promocional do produto em dólares americanos.  
**limited_edition** | Indica se o produto é uma edição limitada ou não (1-verdadeiro, 0-falso).  
**new** | Indica se o produto é novo ou não (1-verdadeiro, 0-falso).  
**online_only** | Indica se o produto é vendido apenas online ou não (1-verdadeiro, 0-falso).  
**out_of_stock** | Indica se o produto está fora de estoque ou não (1 se verdadeiro, 0 se falso).  
**sephora_exclusive** | Indica se o produto é exclusivo da Sephora ou não (1 se verdadeiro, 0 se falso).  
**highlights** | Uma lista de tags ou características que destacam os atributos do produto (ex.: `['Vegano', 'Acabamento Fosco']`).  
**primary_category** | Primeira categoria na seção de navegação do site.  
**secondary_category** | Segunda categoria na seção de navegação do site.  
**tertiary_category** | Terceira categoria na seção de navegação do site.  
**child_count** | O número de variações disponíveis do produto.  
**child_max_price** | O maior preço entre as variações do produto.  
**child_min_price** | O menor preço entre as variações do produto.  

---

### Conteúdo do Dataset_Reviews

**Recurso** | **Descrição**  
--- | ---  
**author_id** | O identificador único do autor da avaliação no site.  
**rating** | A nota dada pelo autor para o produto em uma escala de 1 a 5.  
**is_recommended** | Indica se o autor recomenda o produto ou não (1-verdadeiro, 0-falso).  
**helpfulness** | A proporção de todas as avaliações em relação às avaliações positivas para a resenha: `helpfulness = total_pos_feedback_count / total_feedback_count`.  
**total_feedback_count** | O número total de feedbacks (avaliações positivas e negativas) deixados pelos usuários para a resenha.  
**total_neg_feedback_count** | O número de usuários que deram uma avaliação negativa para a resenha.  
**total_pos_feedback_count** | O número de usuários que deram uma avaliação positiva para a resenha.  
**submission_time** | Data em que a avaliação foi publicada no site no formato 'aaaa-mm-dd'.  
**review_text** | O texto principal da resenha escrito pelo autor.  
**review_title** | O título da resenha escrito pelo autor.  
**skin_tone** | O tom de pele do autor (ex.: clara, morena, etc.).  
**eye_color** | A cor dos olhos do autor (ex.: castanho, verde, etc.).  
**skin_type** | O tipo de pele do autor (ex.: mista, oleosa, etc.).  
**hair_color** | A cor do cabelo do autor (ex.: castanho, ruivo, etc.).  
**product_id** | O identificador único do produto no site.  

🎯 Objetivos

Explorar e analisar avaliações dos clientes.

Aplicar NLP (Processamento de Linguagem Natural) para pré-processamento dos textos.

Desenvolver um modelo de Machine Learning para classificar as avaliações.

Avaliar a performance do modelo com acurácia, precisão, recall e F1-score.

Gerar insights para aprimorar a experiência do consumidor.

🛠 Tecnologias Utilizadas

Python, Pandas, NumPy

NLTK, SpaCy (NLP)

PyTorch (Machine Learning)

Matplotlib, Seaborn (Visualização de dados)

