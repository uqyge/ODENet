# ODENet model for combustion 

ODENetMoel example
```
from ODENet import ODENetModel
dim_input = x_train.shape[1]
dim_label = y_train.shape[1]


model = ODENetModel(
    dim_input=dim_input,
    dim_label=dim_label,
)
model.summary()

loss_type = "mse"
model.compile(loss=loss_type, optimizer="adam", metrics=["accuracy"])
model.fit(x_train,y_train)
```