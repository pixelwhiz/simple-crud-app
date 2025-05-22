## Table of Contents

- [Features](#features)
- [Tech Stack](#tech_stack)
  - [Frontend](#tech_stack_frontend)
  - [Backend](#tech_stack_backend)
  - [Database](#tech_stack_database)
- [Models](#models)

# Features <a name="features"></a>
- [x] **Jwt Auth** - Handle user authentication (Login, Logout)
- [x] **CRUD** - Create, Read, Update, Delete (Siswa)
- [x] **Database** - Save siswa data / model to Database (Data Saving)

# Tech Stack <a name="tech_stack"></a>
### Frontend <a name="tech_stack_frontend"></a>
- Typescript (frontend language)
- React (frontend framework)
- Tailwindcss (css framework)
- Chakra UI (tailwindcss components)

### Backend <a name="tech_stack_backend"></a>
- Golang (backend language)
- Gin (backend framework)

### Database <a name="tech_stack_backend"></a>
- MySQL

# Models <a name="models"></a>
Model `api/models/SiswaModel.go`
```go
type Siswa struct {
	NIS         string    `gorm:"primaryKey" json:"nis"`
	Name        string    `gorm:"type:varchar(191);not null" json:"name"`
	Gender      string    `gorm:"column:gender;type:varchar(191);not null" json:"gender"`
	Address     string    `gorm:"type:varchar(191);not null" json:"address"`
	PhoneNumber string    `gorm:"type:varchar(20);not null" json:"phone_number"`
}
```
