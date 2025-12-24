# SnowShader
Шейдер снега для Unity HDRP/Shader Graph.

## Особенности
- Деформация снега на основе Render Texture.
- Совместимость с High Definition Render Pipeline (HDRP).
- Настраиваемые параметры:
  
<br/>
Main Texture - основная текстура снега. <br/>
Metallic - металик <br/>
Main Texture Tiling - тайлинг MainTexture <br/>
Bottom Color - цвет нижней части снега при деформации. <br/>
Normal Texture - текстура нормали снега. <br/>
NormalMap Tiling - тайлинг NormalMap. <br/>
Normal Stength - сила карты нормали. <br/>
HeightMap - карта высот (текстура) для деформации (RenderTexture). <br/>
Height Multiplier - высота снега. <br/>
BottomHeight - переменная для определения высоты цвета при деформации. <br/>
Edge Fade Start - в процессе. <br/>
Edge Fade End - в процессе. <br/>
Splat Dissolve - переменная для размытия границ при деформации. В основном в диапазоне [0,1] <br/>
Smoothness Texture - текстура Smoothness. <br/>
Smoothness Tiling - тайлинг для Smoothness Texture. <br/>
Smoothness Strength - в процессе. <br/>
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
Main Texture - the main texture of snow. <br/>
Metallic - metallic <br/>
Main Texture Tiling - tiling MainTexture <br/>
Bottom Color - the color of the lower part of the snow during deformation. <br/>
Normal Texture - the texture of the snow normality. <br/>
NormalMap Tiling - tiling NormalMap. <br/>
Normal Stength - the strength of the normal card. <br/>
HeightMap is a height map (texture) for the deformation (RenderTexture). <br/>
Height Multiplier - the height of the snow. <br/>
BottomHeight is a variable for determining the height of a color during deformation. <br/>
Edge Fade Start is in progress. <br/>
Edge Fade End is in progress. <br/>
Splat Dissolve is a variable for blurring borders during deformation. Mostly in the range of [0.1] <br/>
Smoothness Texture - texture of Smoothness. <br/>
Smoothness Tiling - tiling for Smoothness Texture. <br/>
Smoothness Strength is in progress. <br/>
Tesselation Factor - the power of tessellation. <br/>

# Warnings
For the shader to work correctly, the brush texture must use a Wrap Mode other than Repeat, and it must not touch its own edges. The background of the brush should be white.
