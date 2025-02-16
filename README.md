Function TextToColorWave(Wave/T InputWave)
    
    Variable waveSize = DimSize(InputWave, 0)
    Make/D/O/N=(waveSize) ColorWaveUnscaled = StringCRC(0, InputWave[p])
    Make/D/O/N=(waveSize) ColorWave = ColorWaveUnscaled / WaveMax(ColorWaveUnscaled)
    
End
