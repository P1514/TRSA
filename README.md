# TRSA

V 1.0

# Grupos

## Navigation
* Alexandre Dias
* Marco Alb.
* David
* Emanuel
* Pedro

## Perception
* Ricardo Torres
* Ricardo Mota
* Zé Pinto
* João Fernandes
* Beatriz

## Storage/Planner
* Rafael
* Marco Correia
* Ricardo Bel.
* João Ramos
* Guilherme
* Tiago Carrasqueira

# Navigation

* Trajetória
* Localização
* Mapeamento
* Deteção de Obstáculos

# Perception
* Simbolos (2D)
* Objetos (3D)

# Storage Supervisor
* Inventário
* Gestão de Tarefas

# Produtos
* Square
* Triangle
* Dot

# ROS Service - Passos
1.	Supervisor envia mapeamento para ‘/kelp/product_mapping’ 
2.	Nav trata de descobrir a localização do Robo
3.	Nav envia o robô para o inicio da parteleira
4.	Perception verifica parteleira
5.	Acaba a perceção
6.	Planner envia info para a navegação e para o supervisor para tratar da próxima peça
7.	Supervisor cria o planeamento para o trabalhador

# Tópicos

* '/planner/supervisor' , us

* '/planner/navigation' , coordenadas (absolutas), direção (º)

* '/planner/perception' , Ligar 3D, Ligar 2D 

# Pedir
* 'nav->planner' mapa, coordenadas (absolutas), direção (º)

* 'perception->planner' Existe parteleira e qual o lado, Objetos que estão dentro da parteleira

