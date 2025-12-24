# SnowShader

Шейдер снега для Unity HDRP/Shader Graph.

## Особенности

- Деформация снега на основе Render Texture.
- Совместимость с High Definition Render Pipeline (HDRP).
- Настраиваемые параметры:
MainTexture - основная текстура снега.
Metallic - металик
BaseMapTiling - тайлинг MainTexture
Bottom Color - цвет нижней части снега при деформации.
Normal Texture - текстура нормали снега.
NormalMapTiling - тайлинг NormalMap.
NormalStength - сила карты нормали.
HeightMap - карта высот (текстура) для деформации (RenderTexture).
HeightMultiplier - высота снега.
BottomHeight - переменная для определения высоты цвета при деформации.
EdgeFadeStart - в процессе.
EdgeFadeEnd - в процессе.
Splat Dissolve - переменная для размытия границ при деформации. В основном в диапазоне [0,1]
Noise Texture - текстура шума.
Noise Tiling - тайлинг для Noise Texture.
Noise Sparkling - в процессе.
Tesselation Factor - сила тесселяции.

## Скриншоты

![Пример снега на объекте](Screenshots/Example1.png)  
![Снег на террейне](Screenshots/example2.png)

# Предупреждения

Для корректной работы шейдера текстура кисти должна использовать Wrap Mode, отличный от Repeat, и не должна касаться своих собственных краев. Background кисти должен быть белым.

For the shader to work correctly, the brush texture must use a Wrap Mode other than Repeat, and it must not touch its own edges. The background of the brush should be white.
