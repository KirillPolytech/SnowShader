# SnowShader
Шейдер снега для Unity HDRP/Shader Graph.

## Особенности
- Деформация снега на основе Render Texture.
- Совместимость с High Definition Render Pipeline (HDRP).
- Настраиваемые параметры:
  
<br/>
MainTexture - основная текстура снега. <br/>
Metallic - металик <br/>
BaseMapTiling - тайлинг MainTexture <br/>
Bottom Color - цвет нижней части снега при деформации. <br/>
Normal Texture - текстура нормали снега. <br/>
NormalMapTiling - тайлинг NormalMap. <br/>
NormalStength - сила карты нормали. <br/>
HeightMap - карта высот (текстура) для деформации (RenderTexture). <br/>
HeightMultiplier - высота снега. <br/>
BottomHeight - переменная для определения высоты цвета при деформации. <br/>
EdgeFadeStart - в процессе. <br/>
EdgeFadeEnd - в процессе. <br/>
Splat Dissolve - переменная для размытия границ при деформации. В основном в диапазоне [0,1] <br/>
Noise Texture - текстура шума. <br/>
Noise Tiling - тайлинг для Noise Texture. <br/>
Noise Sparkling - в процессе. <br/>
Tesselation Factor - сила тесселяции. <br/>
 
## Скриншоты
<img src="Screenshots/Example1.png" width="500" />
<img src="Screenshots/Example2.png" width="500" />

# Предупреждения
Для корректной работы шейдера текстура кисти должна использовать Wrap Mode, отличный от Repeat, и не должна касаться своих собственных краев. Background кисти должен быть белым.

# ENG
# SnowShader
Snow shader for Unity HDRP/Shader Graph.

## Features
- Snow deformation based on Render Texture.
- Compatible with High Definition Render Pipeline (HDRP).
- Configurable parameters:
<br/>
MainTexture - the main texture of snow. <br/>
Metallic - metallic <br/>
BaseMapTiling - tiling MainTexture <br/>
Bottom Color - the color of the lower part of the snow during deformation. <br/>
Normal Texture - the texture of the snow normality. <br/>
NormalMapTiling - NormalMap tiling. <br/>
NormalStength - the strength of the normal map. <br/>
HeightMap is a height map (texture) for the deformation (RenderTexture). <br/>
HeightMultiplier - the height of the snow. <br/>
BottomHeight is a variable for determining the height of a color during deformation. <br/>
EdgeFadeStart is in progress. <br/>
EdgeFadeEnd is in progress. <br/>
Splat Dissolve is a variable for blurring borders during deformation. Mostly in the range of [0.1] <br/>
Noise Texture - noise texture. <br/>
Noise Tiling - tiling for Noise Texture. <br/>
Noise Sparkling is in progress. <br/>
Tesselation Factor - the power of tessellation. <br/>

# Warnings
For the shader to work correctly, the brush texture must use a Wrap Mode other than Repeat, and it must not touch its own edges. The background of the brush should be white.
