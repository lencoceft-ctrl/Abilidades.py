# --- SISTEMA DE HABILIDADES DO DIGIMUNDO ---

habilidades = {
    "Qi-mon": {
        "ataque": "Bolhas de Pixel",
        "efeito": "Recuo leve",
        "dano": 1
    },
    "Queiro-mon": {
        "ataque": "Brisa Ofuscante",
        "efeito": "Cegueira (Blindness)",
        "duracao_efeito": "3 segundos",
        "descricao": "Uma rajada de pixels de vento que ofusca o inimigo."
    },
    "NaturePatamon": {
        "ataque": "Mini Tornado",
        "defesa": "Antena de Planta (Escudo Orgânico)",
        "especial": "Purificação de Dados"
    }
}

def usar_habilidade(personagem):
    if personagem in habilidades:
        hab = habilidades[personagem]
        print(f"--- {personagem} em combate! ---")
        print(f"Usou: {hab['ataque']}")
        if "efeito" in hab:
            print(f"Efeito ativado: {hab['efeito']}")
    else:
        print("Personagem ainda não registrado no sistema.")

# Testando o sistema
usar_habilidade("Queiro-mon")


____________________________________________________


import math

def calcular_vibracao(tempo_atual, intensidade=2):
    # Usamos o SENO para criar um movimento de vai-e-vem suave
    # Isso faz o ovo vibrar em torno do centro (X=5)
    vibracao = math.sin(tempo_atual * 20) * intensidade
    return vibracao

# No Dia 13, o GDevelop vai somar esse valor à posição X do ovo


