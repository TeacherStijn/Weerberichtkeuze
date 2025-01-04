# Weerberichtkeuze

If(
    MSNWeather.TodaysForecast(
        "Veenendaal",
        "C"
    ).responses.daily.precip > 80,
    regen,
    If(
        MSNWeather.TodaysForecast(
            "Veenendaal",
            "C"
        ).responses.daily.tempLo > 17,
        zon,
        herfst
    )
)
