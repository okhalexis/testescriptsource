--[[
    HUB DE SCRIPTS - ORION LIBRARY MODIFICADA
    Carregando a biblioteca com sistema de pesquisa na Sidebar
]]

local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/okhalexis/source/refs/heads/main/trse1')))()

-- Criando a Janela Principal
local Window = OrionLib:MakeWindow({
    Name = "Roblox Leaks/Scripts HUB",
    HidePremium = false,
    SaveConfig = true,
    ConfigFolder = "OrionHubConfig",
    IntroEnabled = true,
    IntroText = "Carregando Hub..."
})

-- =================================================================
-- CATEGORIA 1: Break a Lucky Block
-- =================================================================

local LuckyBlockTab = Window:MakeTab({
	Name = "Break a Lucky Block",
	Icon = "rbxassetid://4483345998", -- Ícone de Pasta (Genérico)
	PremiumOnly = false
})

LuckyBlockTab:AddSection({
	Name = "Scripts Disponíveis"
})

-- Script: TORA ISME
LuckyBlockTab:AddButton({
	Name = "TORA ISME",
	Callback = function()
        -- Executa o script do Tora Isme
        loadstring(game:HttpGet("https://raw.githubusercontent.com/gumanba/Scripts/main/BreakaLuckyBlock"))()
  	end    
})

-- =================================================================
-- CATEGORIA 2: Escape Tsunami for Brainrots
-- =================================================================

local TsunamiTab = Window:MakeTab({
	Name = "Escape Tsunami for Brainrots",
	Icon = "rbxassetid://4483345998", -- Ícone de Pasta (Genérico)
	PremiumOnly = false
})

TsunamiTab:AddSection({
	Name = "Scripts Disponíveis"
})

-- Script: KLS HUB
TsunamiTab:AddButton({
	Name = "KLS HUB",
	Callback = function()
        -- Executa o script do KLS HUB
        loadstring(game:HttpGet("https://raw.githubusercontent.com/okhalexis/khalexishub/refs/heads/main/10k"))()
  	end    
})

-- =================================================================
-- FINALIZAÇÃO
-- =================================================================

-- Inicializa a interface e notificações
OrionLib:Init()

OrionLib:MakeNotification({
	Name = "Hub Carregado!",
	Content = "Use a barra lateral para pesquisar os jogos.",
	Image = "rbxassetid://4483345998",
	Time = 5
})
