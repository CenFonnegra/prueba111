```mermaid
graph LR
    User((Usuario / Viajero))

    subgraph Sistema Arcoins
        UC1[Registrarse e Iniciar Sesión]
        UC2[Consultar Saldos Multidivisa COP/USD/EUR]
        UC3[Comprar, Vender e Intercambiar Monedas]
        UC4[Consultar Historial con Filtros]
        UC5[Recibir Correo de Confirmación AWS SES]
        UC6[Interactuar con el Asistente IA Gemini]
        UC7[Calcular Presupuesto de Viaje - Adicional]
    end

    User --> UC1
    User --> UC2
    User --> UC3
    User --> UC4
    User --> UC5
    User --> UC6
    User --> UC7