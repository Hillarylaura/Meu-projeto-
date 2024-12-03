def introducao():
    print("Bem-vindo(a) ao Mistérios de Umbra!")
    print("Você é um(a) jovem aprendiz de magia que se perdeu em uma floresta encantada.")
    print("Uma tempestade mágica o(a) arrastou para este lugar. Agora, você precisa escapar.")
    print("Escolha com sabedoria, pois suas decisões determinarão seu destino!\n")
    primeira_escolha()

def primeira_escolha():
    print("Você encontra dois caminhos: ")
    print("1. Um caminho iluminado por luzes dançantes.")
    print("2. Um caminho escuro e silencioso.")
    escolha = input("Qual caminho você escolhe? (1/2): ")
    
    if escolha == "1":
        luzes_dancantes()
    elif escolha == "2":
        caminho_escuro()
    else:
        print("Escolha inválida. Tente novamente.\n")
        primeira_escolha()

def luzes_dancantes():
    print("\nVocê segue as luzes e encontra uma bruxa mística.")
    print("Ela oferece ajuda, mas pede algo em troca.")
    print("Você aceita a oferta da bruxa?")
    escolha = input("(sim/não): ")
    
    if escolha.lower() == "sim":
        final_bom()
    else:
        final_ruim()

def caminho_escuro():
    print("\nVocê escolhe o caminho escuro, mas logo percebe que se perdeu.")
    print("A escuridão é perturbadora, e você não consegue encontrar a saída.")
    final_ruim()

def final_bom():
    print("\nParabéns! Você ganhou a confiança da bruxa.")
    print("Ela revela o caminho para fora da floresta mágica.")
    print("Você escapa com novos conhecimentos e habilidades mágicas!")
    print("Fim do jogo - Final Feliz!")

def final_ruim():
    print("\nInfelizmente, sua jornada termina aqui.")
    print("Você ficou preso(a) na floresta mágica para sempre.")
    print("Fim do jogo - Final Ruim.")

# Inicia o jogo
if __★__ == "__main__":
    introducao()
