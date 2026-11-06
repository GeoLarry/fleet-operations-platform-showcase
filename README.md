# Fleet operations platform — screenshots

A fleet operations platform for leasing and rental companies (own product). Staff record vehicle deliveries and pickups with a full inspection: an interactive car diagram for marking damages, accessories, fuel and mileage, and the customer's e-signature. Each movement produces a PDF report and a notification.

This is a private product, and its source code is not public. This repository only holds screenshots of the running app, with fake demo data. A demo is available on request.

## Features

- Vehicle delivery and pickup with an interactive car diagram for marking damages
- Customer e-signature, PDF movement reports with notifications
- Damage lifecycle: active or repaired, billable or not, with history kept on past movements
- Fleet status views, add and edit vehicles
- User, role and permission administration
- Greek/English UI, dark mode, draft autosave

## Tech stack

| Part | Technologies |
|---|---|
| Frontend | Angular, Angular Material, Greek/English i18n, dark mode |
| Backend | .NET 10 Minimal API, JWT, permission-based authorization, Dapper over SQL Server |
| Reports | Server-side PDF generation |

## Movements

Movements list with search by license plate and date range. The actions on each row depend on the movement's state: open movements can be edited or deleted, completed ones can only be viewed or printed.

![Movements list](screenshots/01-movements-list.png)

The inspection form: general information, damages, accessories, notes and the customer's signature.

![Movement inspection form](screenshots/02-movement-inspection-form.png)

Damages are marked on a diagram of the vehicle and listed with their type, severity and billing.

![Damage diagram](screenshots/03-damage-diagram.png)

Choosing a vehicle zone and the exact area of a new damage.

![Damage zone picker](screenshots/04-damage-zone-picker.png)

A completed movement opens read-only. It keeps the damages that were active at that time, even if they were repaired later.

![Completed movement preview](screenshots/05-completed-movement-preview.png)

Starting a new movement from a license plate (check-in or check-out), and finding a vehicle to manage its damages.

![New movement dialog](screenshots/06-new-movement-dialog.png)
![Damage management search](screenshots/07-damage-management-search.png)

## Fleet

![Fleet list](screenshots/08-fleet-list.png)

Vehicle details, editing and adding a new vehicle.

![Vehicle details](screenshots/09-vehicle-details.png)
![Vehicle edit](screenshots/10-vehicle-edit.png)
![New vehicle](screenshots/11-vehicle-new.png)

Damages belong to the vehicle. They can be recorded and marked as repaired from the fleet view as well, not only through a movement.

![Vehicle damages](screenshots/12-vehicle-damages.png)

## Users and roles

![Users](screenshots/13-users.png)
![User edit](screenshots/14-user-edit.png)

Custom roles grant permissions per module and action.

![Roles](screenshots/15-roles.png)
![Role permissions](screenshots/16-role-permissions.png)

## Dark mode

![Movements list, dark mode](screenshots/17-movements-list-dark.png)
![Movement inspection form, dark mode](screenshots/18-movement-inspection-form-dark.png)
![Fleet list, dark mode](screenshots/19-fleet-list-dark.png)
